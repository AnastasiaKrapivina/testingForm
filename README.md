### 1. Перечень автоматизируемых сценариев:
#### 1. Переход в раздел формы записи на обучение с главной страницы:
- Вариант 1. Через "Каталог курсов" и "Курсы для новичков" используя верхнюю кнопку "Записаться":<br>
Вход на сайт https://netology.ru/  -> Меню "Каталог курсов" ->  "Курсы для новичков" -> Тестировщик ПО ->  "Записаться"(кнопка вверху страницы) ->"Записаться"(кнопка внизу страницы)<br>
- Вариант 2. Через "Каталог курсов" и "Полный каталог" используя верхнюю кнопку "Записаться": <br>
Вход на сайт https://netology.ru/  -> Меню "Каталог курсов" ->  "Полный каталог" -> Тестировщик ПО->  "Записаться"(кнопка вверху страницы) ->"Записаться"(кнопка внизу страницы)<br>
- Вариант 3. Через контент на главной странице "Курсы для новичков" используя верхнюю кнопку "Записаться":<br>
Вход на сайт https://netology.ru/  -> Контент на главной странице "Курсы для новичков"  ->Тестировщик ПО->  "Записаться"(кнопка вверху страницы) ->"Записаться"(кнопка внизу страницы)<br>
- Вариант 4. Через "Каталог курсов" и "Курсы для новичков" используя только нижнюю кнопку "Записаться":<br>
Вход на сайт https://netology.ru/  -> Меню "Каталог курсов"  ->  "Курсы для новичков" -> Тестировщик ПО  -> "Пролистать всю страницу профессии" -> "Записаться"(кнопка внизу страницы)<br>
- Вариант 5. Через "Каталог курсов" и "Полный каталог" используя только нижнюю кнопку "Записаться":<br>
Вход на сайт https://netology.ru/  -> Меню "Каталог курсов" ->  "Полный каталог" -> Тестировщик ПО -> "Пролистать всю страницу профессии" -> "Записаться"(кнопка внизу страницы)<br>
- Вариант 6. Через контент на главной странице "Курсы для новичков" используя только нижнюю кнопку "Записаться":<br>
Вход на сайт https://netology.ru/  ->Контент на главной странице "Курсы для новичков"  ->Тестировщик ПО-> "Пролистать всю страницу профессии" -> "Записаться"(кнопка внизу страницы)<br>
#### 2. Заполнение формы "Запишитесь на курс":
***Требования к содержимому полей:***<br>
- Поле "Имя": должно состоять из русских и латинских букв, допускаются дефисы и пробелы.<br>
- Поле "Телефон": только 11 цифр, на первом месте или +7 или 8.<br>
- Поле "Электронная почта": в формате username@hostname.domain или ящик@почта.рф. <br>
  Username должен состоит из русских или латинских букв, а так же цифр, может содержать одну точку, за исключением первого и последнего знака, а так же спецсимволы: ! # $ % & ‘ * + — / =? ^ _ ` { | } ~. <br>
  Hostname должен состоят из русских или латинских букв, цифр и дефисов, причём дефисы не могут быть в начале или в конце компонента.<br>
  Domain - ограниченный список доменов первого уровня.<br>

***Предусловие:*** Выполнить "Вариант 1" перехода в раздел формы записи на обучение с главной страницы.<br>

1. **Позитивные кейсы:**<br>
   **Тест 1:** Ввод валидных значений на кирилице в поля "Имя"(Иван),"Электронная почта"(Иван@почта.ру) и "Телефон"(+79999991111). Нажать кнопку "Записаться". <br>
   *Ожидаемый результат:* Система выдает информационное сообщение о том, что заявка на запись принята.<br>
   **Тест 2:** Ввод валидных значений на литинице в поля "Имя"(Ivan), "Электронная почта"(Ivan@mail.ru) и "Телефон"(89999991111). Нажать кнопку "Записаться". <br>
   *Ожидаемый результат:* Система выдает информационное сообщение о том, что заявка на запись принята.<br>
   **Тест 3:** Ввод валидного значения в поля "Имя" на кирилице с буквой "ё" (Артём), "Электронная почта"(Ivan@mail.ru) и "Телефон"(+79999991111). Нажать кнопку "Записаться". <br>
   *Ожидаемый результат:* Система выдает информационное сообщение о том, что заявка на запись принята.<br>
   **Тест 4:** Ввод валидного значения в поля "Имя" на кирилице составного с пробелом (Василий Иван), "Электронная почта"(Ivan@mail.ru) и "Телефон"(+79999991111). Нажать кнопку "Записаться". <br>
   *Ожидаемый результат:* Система выдает информационное сообщение о том, что заявка на запись принята.<br>
   **Тест 5:** Ввод валидного значения в поля "Имя" на кирилице составного с дефисом (Василий-Иван), "Электронная почта"(Ivan@mail.ru) и "Телефон"(+79999991111). Нажать кнопку "Записаться". <br>
   *Ожидаемый результат:* Система выдает информационное сообщение о том, что заявка на запись принята.<br>
   **Тест 6:** Ввод валидных значений в поля "Имя" (Иван), "Электронная почта"  (содержит цифры 1212@1212.ru) и "Телефон"(+79999991111). Нажать кнопку "Записаться". <br>
   *Ожидаемый результат:* Система выдает информационное сообщение о том, что заявка на запись принята.<br>
   **Тест 7:** Ввод валидных значений в поля "Имя" (Иван), "Электронная почта"  (username содержит точку Ivan.An@mail.ru) и "Телефон"(+79999991111). Нажать кнопку "Записаться". <br>
   *Ожидаемый результат:* Система выдает информационное сообщение о том, что заявка на запись принята.<br>
   **Тест 8:** Ввод валидных значений в поля "Имя" (Иван), "Электронная почта"  (username содержит спецсимвол Ivan_An@mail.ru) и "Телефон"(+79999991111). Нажать кнопку "Записаться". <br>
   *Ожидаемый результат:* Система выдает информационное сообщение о том, что заявка на запись принята.<br>
   **Тест 9:** Ввод валидных значений в поля "Имя", "Телефон" и "Электронная почта". Нажать кнопку "Получить консультацию".<br>
   *Ожидаемый результат:* Система выдает информационное сообщение о том, что заявка на получение консультации принята.<br>
   **Тест 10:** Нажатие кнопки "принимаю условия политики"<br>
   *Ожидаемый результат:* переход в раздел сайта "ПОЛИТИКА ОБРАБОТКИ ПЕРСОНАЛЬНЫХ ДАННЫХ ПОЛЬЗОВАТЕЛЕЙ САЙТА".<br>
   **Тест 11:** Нажатие кнопки "пользовательского соглашения"<br>
   *Ожидаемый результат:* переход в раздел сайта "Пользовательское соглашение"<br>
   **Тест 12:** Нажатие кнопки "Уже есть аккаунт? Войти"<br>
   *Ожидаемый результат:* переход на страницу входа в личный кабинет<br>
2. **Негативные кейсы:**<br>
   **Тест 13:** Отправка формы с незаполнеными полями. Оставить поля<br>
   *Ожидаемый результат:* Система выдает информационное сообщение о том, что необходимо заполнить поля формы.<br>
   **Тест 14:** Ввод невалидного значения в поле "Имя" (Я) и валидных значения в поле "Телефон" и "Электронная почта". Нажать кнопку "Записаться"<br>
   *Ожидаемый результат:* Под полем "Имя" появляется предупредительное информационное сообщение, что введено недопустимое значение. Система выдает информационное сообщение о том, что введите допустимые значения в поля формы.<br>
   **Тест 15:** Ввод невалидного значения в поле "Имя" (123) и валидных значения в поле "Телефон" и "Электронная почта". Нажать кнопку "Записаться"<br>
   *Ожидаемый результат:* Под полем "Имя" появляется предупредительное информационное сообщение, что введено недопустимое значение. Система выдает информационное сообщение о том, что введите допустимые значения в поля формы.<br>
   **Тест 16:** Ввод валидных значений в поля "Имя" и "Электронная почта", а так же невалидного значения в поле "Телефон"(000000000). Нажать кнопку "Записаться"<br>
   *Ожидаемый результат:* Под полем "Телефон" появляется предупредительное информационное сообщение, что введено недопустимое значение. Система выдает информационное сообщение о том, что введите допустимые значения в поля формы.<br>
   **Тест 17:** Ввод валидных значений в поля "Имя" и "Электронная почта", а так же невалидного значения в поле "Телефон"(812345678912345). Нажать кнопку "Записаться"<br>
   *Ожидаемый результат:* Под полем "Телефон" появляется предупредительное информационное сообщение, что введено недопустимое значение. Система выдает информационное сообщение о том, что введите допустимые значения в поля формы.<br>
   **Тест 18:** Ввод валидных значений в поля "Имя", "Телефон" и невалидного значения в поле "Электронная почта"(Ivan.@mail.ru). Нажать кнопку "Записаться"<br>
   *Ожидаемый результат:* Под полем "Электронная почта" появляется предупредительное информационное сообщение, что введено недопустимое значение. Система выдает информационное сообщение о том, что введите допустимые значения в поля формы.<br>

### 2. Перечень используемых инструментов с обоснованием выбора.
1. **Google Chrome**, браузер, для исследования тестируемой страницы
2. **IntelliJ IDEA**,среда разработки для создания проекта
3. **Java Development Kit 11**, набор инструментов для разработки на языке Java 
4. **Gradle**, система для автоматизации сборки приложений и сбора статистики об использовании программных библиотек, применяющая язык Java
5. **Selenide**, для тестирования веб-интерфейсов, представляет собой простое в использовании дополнение к браузеру Chrome и путем имитации действий пользователя происходит составление сценариев для тестов
6. **JUnit 5**, среда тестирования для приложений Java
7. **Datafaker**, для генерации фиктивных данных, похожих на производственные данные
8. **Lombok**, основанная на аннотациях библиотека Java, позволяющая сократить шаблонный код
9. **Allure Framework**, фреймворк, который служит для получения отчетов о прохождении авто-тестов.

### 3. Перечень необходимых разрешений, данных и доступов.
1. Разрешение на выполнение автоматизированного тестирования у владельца сайта
2. Перечень устройств, на которых необходимо проводить тестирование
3. Список ОС и браузеров для тестирования
4. Разрешения экранов на которых необходимо проверить заполнение формы
5. Есть ли необходимость авторицации пользователя для заполнения формы
6. Доступы к базе данных
7. API сайта

### 4. Перечень и описание возможных рисков при автоматизации.
1. Отсутствие тестовых меток, четкой привязки к элементам
2. Постоянно меняющаяся структура сайта, частое обновление интерфейса
3. Время, затраченное на подготовку автотестов окажется больше, чем на ручное тестирование
4. Стоимость тестирования до автоматизации может быть меньше, чем после внедрения автоматизации.
5. Ввод автотестирования может повлечь за собой зависимость от специалистов нужной квалификации
6. Невозможность все покрыть автотестами, например "Нагрузочное тестирование".

### 5. Перечень необходимых специалистов для автоматизации.
- QA-инженер
### 6. Интервальная оценка с учётом рисков в часах.
1. Подготовка тестовых сценариев - 8 часов.
2. Написание автотестов, тестирование и отладка автотестов - 32 часов.
3. Подготовка отчетов - 8 часов