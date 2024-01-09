#Эта программа создана для осуществления парсинга
из заранее определенного списка компаний и их открытых вакансий
на сайте HeadHunter.ru

#Полученные результаты заносятся в базу данных SQL

#Перед началом работы с программой необходимо
зарегистрироваться на PostgreSQL, создать виртуальное окружение Poetry

#Перед запуском программы надо заполнить файл database.ini, где указать:
user=<Ваше имя пользователя>
password=<Ваш пароль при регистрации в postgres>
port=<по умолчанию <5432> или <5433>, если Вы работает на MacOS

#Все зависимости находятся в файле pyproject.toml

##Программа запускается из файла main.py

###При запуске программы происходит запрос с сайта НН по компаниям:
Яндекс, Россельхозбанк, Сбер, ВТБ,
2Гис, Альфабанк, Газпромбанк, Лукойл,
Яндекс Еда, Автоваз
создается база в sql и две таблицы Дальнейшая работа происходит с базой

###Пользователь может выбрать несколько опций по выводу данных из таблиц и
осуществить поиск вакансий по ключевому слову

###Программа прекращает работу при введении слова "стоп" или "stop"