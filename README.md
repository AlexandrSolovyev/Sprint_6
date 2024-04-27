# Sprint_6

*Проект автоматизации тестирования сайта заказа самокатов https://qa-scooter.praktikum-services.ru/*

1. Основа для написания автотестов — фреймворк pytest, selenium.
2. Для отчетов используется Allure
3. Автотесты написаны в соответствии паттерна POM
4. Установить зависимости — `pip install -r requirements.txt`
5. Команда для запуска — `pytest -v`
6. Команда для запуска с записью отчета в allure_results: `pytest --alluredir=allure_results`
7. Генерация отчета в html страницу (находясь в дирректории allure_results): _`allure serve allure_results`_ 

### Директория проекта:

* `allure_results` - сожержит отчеты alure
 *  `locators` - дирректория локаторов
 * * `main_page_locators.py` - локаторы для главной страницы 
 * * `order_page_locators.py` - локаторы для страницы заказа
 * `pages` - дирректория методов страниц
 * * `base_page.py` - общие методы
 * * `main_page.py` - методы для главной страницы
 * * `order_page.py` - методы для страницы заказа 
 * `tests` - дирректория тестов
 * * `test_main_page.py` - тесты для главной страницы
 * * `test_order_page.py` - тесты для страницы заказа
 * `conftest.py` -  фикстуры
 * `date.py` - данные для параметризации
 * `README.md` - описание проекта
 * `requirements` - файл с внешними зависимостями
 *  `settings` - файл с настраивыми константами