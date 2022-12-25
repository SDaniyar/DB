Домашнее задание 2 

Схема таблиц

<image src="https://github.com/SDaniyar/DB/blob/main/HW2/Diagram1.PNG" alt="Схема">

На примере таблиц Tours, Booking проведем анализ возможных запросов\отчетов\поиска данных, создадим индексы, создадим ограничения.

1. Создадим внешние ключи к связанным таблицам 

<image src="https://github.com/SDaniyar/DB/blob/main/HW2/TOUR_FK.PNG" alt="FK">

2. Создадим первичный ключ (на поле id) и ограничение на цену тура (ALTER TABLE public.tours ADD CONSTRAINT tours_check CHECK (price > 0);)

<image src="https://github.com/SDaniyar/DB/blob/main/HW2/TOUR_PK.PNG" alt="PK">

3. В нашей таблице туров основной поиск будет идти по странам, отбор по цене и датам тура
 - Создаем индекс по странам (county_id)
 - Создаем индекс по цене (price)
 - Создаем индекс по датам тура (start_date end_date)

<image src="https://github.com/SDaniyar/DB/blob/main/HW2/TOUR_Inx.PNG" alt="index">





