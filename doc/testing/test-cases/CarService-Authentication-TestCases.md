### *Страница «Authentication» на сайте CarService*

---

**Name:** #1. Наличие поля «Login» на сайте CarService\
**Preconditions:** Пользователь находится на странице «Authentication» на сайте CarService\
**Step 1:** Checking страницы «Authentication» на наличие поля «Login»\
**Expected result:** Поле «Login» на странице «Authentication» сайта CarService отображается

---

**Name:** #2. Наличие поля «Password» на сайте CarService\
**Preconditions:** Пользователь находится на странице «Authentication» на сайте CarService\
**Step 1:** Checking страницы «Authentication» на наличие поля «Password»\
**Expected result:** Поле «Password» на странице «Authentication» сайта CarService отображается

---

**Name:** #3. Наличие кнопки «Log in» на сайте CarService\
**Preconditions:** Пользователь находится на странице «Authentication» на сайте CarService\
**Step 1:** Checking страницы «Authentication» на наличие кнопки «Log in»\
**Expected result:** Кнопка «Log in»  на странице «Authentication» сайта CarService отображается

---

**Name:** #4. Доступность аутентификации на сайте CarService с корректными Login и Password\
**Preconditions:** Пользователь находится на странице «Authentication» на сайте CarService. Поля «Login», «Password» и кнопка «Log in» отображаются на сайте.\
**Step 1:** Ввести в поля ввода Login и Password корректные значения. Нажать на кнопку «Log in»\
**Expected result:** Пользователь перенаправляется на главную страницу сайта. Появляется оповещение, что пользователь уже залогинен.

---

**Name:** #5. Недоступность регистрации на сайте CarService с некорректным Login и корректным Password\
**Preconditions:** Пользователь находится на странице «Authentication» на сайте CarService. Поля «Login», «Password» и кнопка «Log in» отображаются на сайте.\
**Step 1:**\
    Ввести в поле ввода Login некорректное значение:\
        • несуществующий Login\
        • символы "«»№;%\~@#$%^&\*(){}[].,<>/\\\
        • пробелы\
        • оставить поле Login пустым\
    В поле ввода Password ввести корректное значение. Нажать на кнопку «Log in»\
**Expected result:** Пользователь остается на текущей странице сайта. Появляется уведомление о некорректно введенных Login/Password.

---

**Name:** #6. Недоступность регистрации на сайте CarService с корректным Login и некорректным Password\
**Preconditions:** Пользователь находится на странице «Authentication» на сайте CarService. Поля «Login», «Password» и кнопка «Log in» отображаются на сайте.\
**Step 1:**\
    Ввести в поле ввода Login корректное значение.\
    В поле ввода Password ввести некорректное значение:\
        • символы "«»№;%\~@#$%^&\*(){}[].,<>/\\\
        • оставить поле Password пустым\
        • пробелы\
        • количество символов не входит в допустимые границы (6<=n<=64)\
    Нажать на кнопку «Log in»\
**Expected result:** Пользователь остается на текущей странице сайта. Появляется уведомление о некорректно введенных Login/Password.

---

**Name:** #7. Недоступность регистрации на сайте CarService с некорректными Login и Password\
**Preconditions:** Пользователь находится на странице «Authentication» на сайте CarService.  Поля «Login», «Password» и кнопка «Log in» отображаются на сайте.\
**Step 1:**\
    Ввести в поле ввода Login некорректное значение:\
        • несуществующий Login\
        • символы "«»№;%\~@#$%^&\*(){}[].,<>/\\\
        • пробелы\
        • оставить поле Login пустым\
    В поле ввода Password ввести некорректное значение:\
        • символы "«»№;%\~@#$%^&\*(){}[].,<>/\\\
        • оставить поле Password пустым\
        • пробелы\
        • количество символов не входит в допустимые границы (6<=n<=64)\
    Нажать на кнопку «Log in»\
**Expected result:** Пользователь остается на текущей странице сайта. Появляется уведомление о некорректно введенных Login/Password.
