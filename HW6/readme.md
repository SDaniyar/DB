Домашнее задание 6

БД Туристического агенства 

Используем БД которую создали ранее


Создадим новый индекс для таблицы tours по полю цена (price). Ожидаем что поиск будет происходить по цене тура. 

<image src="https://github.com/SDaniyar/DB/blob/main/HW6/IND1.PNG" alt="index">

Текст результат команды explain

<image src="https://github.com/SDaniyar/DB/blob/main/HW6/IND2.PNG" alt="index">

Реализуем индекс для полнотекстового поиска. Для полноценного поиска по комментариям, используем полнотекстовый поиск. 

<image src="https://github.com/SDaniyar/DB/blob/main/HW6/IND3.PNG" alt="index">

Реализуем индекс на часть таблицы. Для уменьшение размера индекса, исключим поля старее '2020-01-01'

<image src="https://github.com/SDaniyar/DB/blob/main/HW6/IND4.PNG" alt="index">

Реализуем составной индекс на полям дат. Для поиска по 2 дата одновременно. 

<image src="https://github.com/SDaniyar/DB/blob/main/HW6/IND5.PNG" alt="index">


Проблемы

Не было данных в своей БД для тестирования индекса. Внес данные. 

PgAdmin показался более удобен для выполнения команды explain нежели dbeaver.

При реализации полнотекстового индекса были проблемы. Подключил расширения 

CREATE EXTENSION pg_trgm; 
CREATE EXTENSION btree_gin;

