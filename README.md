### 1. Перечень автоматизируемых сценариев:
#### 1. Переход в раздел формы записи на обучение с главной страницы:
- Вход на сайт https://netology.ru/  -> Меню "Каталог курсов" ->  "Курсы для новичков" -> Тестировщик ПО ->  "Записаться"(кнопка вверху страницы) ->"Записаться"(кнопка внизу страницы)
- Вход на сайт https://netology.ru/  -> Меню "Каталог курсов" ->  "Полный каталог" -> Тестировщик ПО->  "Записаться"(кнопка вверху страницы) ->"Записаться"(кнопка внизу страницы)
- Вход на сайт https://netology.ru/  -> Контент на главной страниц "Курсы для новичков"  ->Тестировщик ПО->  "Записаться"(кнопка вверху страницы) ->"Записаться"(кнопка внизу страницы)
- Вход на сайт https://netology.ru/  -> Меню "Каталог курсов"  ->  "Курсы для новичков" -> Тестировщик ПО  -> "Пролистать всю страницу профессии" -> "Записаться"(кнопка внизу страницы)
- Вход на сайт https://netology.ru/  -> Меню "Каталог курсов" ->  "Полный каталог" -> Тестировщик ПО -> "Пролистать всю страницу профессии" -> "Записаться"(кнопка внизу страницы)
- Вход на сайт https://netology.ru/  ->Контент на главной страниц "Курсы для новичков"  ->Тестировщик ПО-> "Пролистать всю страницу профессии" -> "Записаться"(кнопка внизу страницы)
#### 2. Тестирование формы "Запишитесь на курс":
- Ввод валидных значений в поля "Имя", "Телефон" и "Электронная почта"
- Ввод невалидного значения в поле "Имя" и валидных значения в поле "Телефон" и "Электронная почта"
- Ввод валидных значений в поля "Имя" и "Электронная почта", а так же невалидного значения в поле "Телефон"
- Ввод валидных значений в поля "Имя", "Телефон" и невалидного значения в поле "Электронная почта"
- Отправка формы с валидными значениями полей
- Оправка формы с невалидними значениями полей
- Переход во вкладку "Получить консультацию"
- Нажатие кнопки "принимаю условия политики"
- Нажатие кнопки "пользовательского соглашения"
- Нажатие кнопки "Уже есть аккаунт? Войти"

### 2. Перечень используемых инструментов с обоснованием выбора.
1. **IntelliJ IDEA**,среда разработки для создания проекта
2. **Gradle**, система для автоматизации сборки приложений и сбора статистики об использовании программных библиотек, применяющая язык Java
3. **Selenide**, для тестирования веб-интерфейсов, представляет собой простое в использовании дополнение к браузеру Chrome и путем имитации действий пользователя происходит составление сценариев для тестов
4. **JUnit 5**, среда тестирования для приложений Java
5. **Datafaker**, для генерации фиктивных данных, похожих на производственные данные
6. **Lombok**, основанная на аннотациях библиотека Java, позволяющая сократить шаблонный код
7. **Allure Framework**, фреймворк, который служит для получения отчетов о прохождении авто-тестов.

### 3. Перечень необходимых разрешений, данных и доступов.
1. Перечень устройств, на которых необходимо проводить тестирование
2. Список ОС и браузеров для тестирования
3. Разрешения экранов на которых необходимо проверить заполнение формы
4. Есть ли необходимость авторицации пользователя для заполнения формы

### 4. Перечень и описание возможных рисков при автоматизации.
1. Стоимость тестирования до автоматизации может быть меньше, чем после внедрения автоматизации.
2. Ввод автотестирования может повлечь за собой зависимость от специалистов нужной квалификации
3. Время, затраченное на подготовку автотестов окажется больше, чем на ручное тестирование.
4. Невозможность все покрыть автотестами, например "Нагрузочное тестирование".

### 5. Перечень необходимых специалистов для автоматизации.
- QA-инженер
### 6. Интервальная оценка с учётом рисков в часах.
1. Подготовка тестовых сценариев - 8 часов.
2. Написание автотестов, тестирование и отладка автотестов - 32 часов.
3. Подготовка отчетов - 8 часов