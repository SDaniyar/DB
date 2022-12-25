Домашнее задание 2 

Схема таблиц

<image src="https://github.com/SDaniyar/DB/blob/main/HW2/Diagram1.PNG" alt="Схема">

На примере таблиц Tours, Booking проведем анализ возможных запросов\отчетов\поиска данных, создадим индексы, создадим ограничения.

1. Создадим внешние ключи к связанным таблицам 

<image src="https://github.com/SDaniyar/DB/blob/main/HW2/TOUR_FK.PNG" alt="FK">

2. Создадим первичный ключ и ограничение на цену тура

image src="https://github.com/SDaniyar/DB/blob/main/HW2/TOUR_PK.PNG" alt="PK">

3.



ALTER TABLE public.tours ADD CONSTRAINT tours_check CHECK (price > 0);




