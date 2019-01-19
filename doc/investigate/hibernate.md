# Hibernate to test:

- check insert and delete sql

- lazy and join selects for one entity

- one-to-many selects

- many-to-one selects

- limit (offset, rowcount)

- order by (asc, desc)

- date / time

- count of related elements

- many-to-many relations

- group by:
<pre>
    <entry key="getMostUsedTags">
        select
            tags.tag_id,
            tags.tag_text,
            count(posts_tags.tag_id) links
        from tags left join posts_tags
            using (tag_id)
        where
            tags.tag_id > :maxSkipId
        group by
            tags.tag_id
        order by
            links desc,
            tags.tag_id
        limit :limit
    </entry>
</pre>

- select inside select:
<pre>
    <entry key="getAdminTagByTagId">
        select
            t.tag_id,
            t.tag_text,
            t.keywords,
            t.description,
            t.admin_comment,
            (SELECT COUNT(*) FROM posts_tags pt WHERE t.tag_id = pt.tag_id) posts_count
        from tags t
        where t.tag_id = :tagId
    </entry>
</pre>
