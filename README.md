## 1.	Перечень автоматизируемых сценариев.

Сценарии навигации к форме:

-	Главная → Направления обучения программирование → Тестировщик ПО → Записаться по кнопке вверху слева.
-	Главная → Каталог курсов → Программирование → Поиск по тексту «тес» → Найти курс → Тестировщик ПО → Записаться справа вверху, рядом с кнопкой авторизации.
-	Главная → Полный каталог → Поиск по тексту «тест» → Найти курс → Тестировщик ПО → Скролл вниз страницы → Записаться 
-	Главная → Каталог курсов → Поиск по тексту «тес» → клик по Тестировщик ПО → Записаться по кнопке вверху слева.
-	Главная → Скролл в подвал → Программирование → Поиск по странице блока «Тестировщик ПО», клик → Записаться справа вверху, рядом с кнопкой авторизации.
-	Главная → Скролл в подвал → Каталог курсов → Поиск по тексту «тес» → клик по Тестировщик ПО → Записаться по кнопке вверху слева.

Сценарии заполнения и отправки формы: 

### Позитивные кейсы

 1. Открыть страницу https://netology.ru/programs/qa#/ 
 2. Заполнить форму валидными данными
 Данные для заполнения формы: имя - Петр, телефон - +7 900 000 00 00, электронная почта - mail@mail.ru
 3. Клик по кнопке "Записаться" 
 ОР: форма успешно заполнена, все поля провалидированы как корректные, заявка отправлена, появилось сообщение: "заявка отправлена в ближайшее время с вами свяжется специалист"
 ---
 1. Открыть страницу https://netology.ru/programs/qa#/ 
 2. Заполнить форму валидными данными
 Данные для заполнения формы: имя - Екатерина, телефон - 8 900 000 00 00, электронная почта - mail@gmail.com
 3. Клик по кнопке "Записаться" 
 ОР: форма успешно заполнена, все поля провалидированы как корректные, заявка отправлена, появилось сообщение: "заявка отправлена в ближайшее время с вами свяжется специалист"
 ---
 1. Открыть страницу https://netology.ru/programs/qa#/ 
 2. Заполнить форму валидными данными
 Данные для заполнения формы: имя - Эмилия-Анна, телефон - 900 000 00 00, электронная почта - mail@ya.ru
 3. Клик по кнопке "Записаться" 
 ОР: форма успешно заполнена, все поля провалидированы как корректные, заявка отправлена, появилось сообщение: "заявка отправлена в ближайшее время с вами свяжется специалист"
  ---
 1. Открыть страницу https://netology.ru/programs/qa#/ 
 2. Заполнить форму валидными данными
 Данные для заполнения формы: имя - Эдриан Анатолий, телефон - +7 900 000 00 00, электронная почта - mail@korpmail.ru
 3. Клик по кнопке "Записаться" 
 ОР: форма успешно заполнена, все поля провалидированы как корректные, заявка отправлена, появилось сообщение: "заявка отправлена в ближайшее время с вами свяжется специалист"
 
 ### Негативные кейсы
  
  Не заполнена почта
  1. Открыть страницу https://netology.ru/programs/qa#/ 
  2. Заполнить поле имя значением "Петр"
  3. Заполнить поле телефон значением "+7 900 000 00 00"
  4. Клик по кнопке "Записаться"
  ОР: заявка не отправлена, поле "Электронная почта" подсвечено красным, под полем сообщение: "поле обязательно для заполнения, укажите адрес вашей электронной почты"
  ---
  Не заполнен телефон
  1. Открыть страницу https://netology.ru/programs/qa#/
  2. Заполнить поле имя значением "Петр"
  3. Заполнить поле "Электронная почта" значением mail@mail.ru
  4. Клик по кнопке "Записаться"
  ОР: заявка не отправлена, поле "Телефон" подсвечено красным, под полем сообщение: "поле обязательно для заполнения, укажите ваш номер телефона"
  ---
  Не заполнено Имя
  1. Открыть страницу https://netology.ru/programs/qa#/
  2. Заполнить поле телефон значением "+7 900 000 00 00"
  3. Заполнить поле "Электронная почта" значением mail@mail.ru
  4. Клик по кнопке "Записаться"
  ОР: заявка не отправлена, поле "Имя" подсвечено красным, под полем сообщение: "поле обязательно для заполнения, укажите ваше Имя"
  ---
  Имя невалидные данные (арабская вязь)
  1. Открыть страницу https://netology.ru/programs/qa#/
  2. Заполнить поле имя значением "عباس"
  3. Заполнить поле телефон значением "+7 900 000 00 00"
  4. Заполнить поле "Электронная почта" значением mail@mail.ru
  5. Клик по кнопке "Записаться"
  ОР: заявка не отправлена, поле "Имя" подсвечено красным, под полем сообщение: "недопустимые символы, допустимые символы — Кириллица и -"
  ---
  Телефон невалидные данные (буквы)
  1. Открыть страницу https://netology.ru/programs/qa#/
  2. Заполнить поле имя значением "Петр"
  3. Заполнить поле телефон значением "khgkydsov"
  4. Заполнить поле "Электронная почта" значением mail@mail.ru
  5. Клик по кнопке "Записаться"
  ОР: заявка не отправлена, поле "Телефон" подсвечено красным, под полем сообщение: "недопустимые символы, телефон может состоять только из цифр"
  ---
  Почта невалидные данные (неправильный формат, без @ и домена)
  1. Открыть страницу https://netology.ru/programs/qa#/
  2. Заполнить поле имя значением "Петр"
  3. Заполнить поле телефон значением "+7 900 000 00 00"
  4. Заполнить поле "Электронная почта" значением email
  5. Клик по кнопке "Записаться"
  ОР: заявка не отправлена, поле "Электронная почта" подсвечено красным, под полем сообщение: "неверный email, формат электронной почты - ***@**.domen"


## 2.	Перечень используемых инструментов с обоснованием выбора.

- Язык программирования Java 8 (объектная ориентация позволяет удобно проектировать классы для тестирования, большое количество библиотек, плагинов и фреймворков, много информации в интернете)
- Среда разработки IntelliJ IDEA (есть бесплатная версия, интеграция с GIT, возможность использовать разные сборки maven, greadle)
-	Сборка на гредл (удобство подключения селениума и CI).
- Junit 5 (удобство в подключении и широкий спектр возможностей для тестирования)
-	Селениум для автоматизации действий на странице. (встроенный webdriver, поддерживает несколько браузеров)
-	CI Allure чтобы следить за прогоном тестов, изучать статистику по итогам. (простота в настройке, в то же время отчеты достаточно информативны)
-	Rest-assured для автоматизации тестирования отправки формы. (проверить разные способы добраться до формы с валидной отправкой, отдельно через API тестировать отправку формы по различным сценариям: валидные и не валидные данные; пользователь, который уже отправлял заявку; пользователь, который уже учится на этом курсе; забаненный пользователь)
-	Docker для базы пользователей, для тестирования отправки формы по API. 

## 3.	Перечень необходимых разрешений, данных и доступов

- Получить разрешение на автоматизацию тестирования сайта
-	Структура базы данных для проверки пользователя (имя, телефон и почта)
-	Документация по API для тестирования отправки формы

## 4.	Перечень и описание возможных рисков при автоматизации.

-	Изменение структуры сайта, расположение кнопок и блоков, участвующих в сценариях перехода до формы заявки.
-	Изменения в названиях разделов и курсов. 

## 5.	Перечень необходимых специалистов для автоматизации.

- QA инженер - автоматизатор. 

## 6.	Интервальная оценка с учётом рисков в часах.

50 часов. 
