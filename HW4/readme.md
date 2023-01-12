Домашнее задание 4 

БД Туристического агенства 

Используем БД которую создали ранее

<image src="https://github.com/SDaniyar/DB/blob/main/HW4/Diagram1.PNG" alt="Схема">

Создаем новую роль 

create role developer1;

Выдаем права на сврю схему 

GRANT ALL PRIVILEGES ON ALL TABLES IN SCHEMA public TO "developer1";

даем права входа

alter role developer1 login;

<image src="https://github.com/SDaniyar/DB/blob/main/HW4/Roles.PNG alt="Схема">

Создаем новую схему private - create schema private;

<image src="https://github.com/SDaniyar/DB/blob/main/HW4/schema.PNG" alt="Схема">


Создаем таблицу managers в новой схеме private

CREATE TABLE private.managers (
	id int4 NOT NULL,
	"name" varchar NULL,
	iin varchar NULL,
	CONSTRAINT managers_pk PRIMARY KEY (id)
);

<image src="https://github.com/SDaniyar/DB/blob/main/HW4/T1.PNG" alt="Схема">