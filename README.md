**Лабораторная работа №1**

Здесь приведены задачи по взаимодействию с таблицей `orders`.

1.  **Получение всех заказов:** Нужно получить все данные из таблицы `orders`.

    [![d9608d10-9358-404a-8b05-6d223a6cfb56](https://github.com/user-attachments/assets/48f3366e-a32e-4ef9-b32d-e2388fdfe10a)
фото 1]

2.  **Исключение новых заказов:** Нужно выбрать все заказы, за исключением тех, у которых статус "new". Используется оператор `IN`.

    [![image](https://github.com/user-attachments/assets/3f1da07d-d8f6-44af-aceb-cfb9b0c8b85f)
фото 2]

3.  **Выбор новых и отмененных заказов:** Необходимо получить список заказов со статусом "new" или "cancelled".

    [blob:https://web.telegram.org/0c1b5caa-30ee-4967-b8ba-069cd6262b0b фото 3]

4.  **Заказы с большим количеством товаров:** Выбираются заказы, где количество товаров (`products_count`) больше 3. Выводятся только идентификатор заказа (`id`) и общая стоимость (`sum`).

    [![image](https://github.com/user-attachments/assets/cf4df78c-daf8-42db-933a-2b13e425ce47)
фото 4]

**Лабораторная работа №2**

Задачи по работе с таблицами `orders` и `products`.

1.  **Три самых дешевых заказа:** Необходимо найти три заказа с самой низкой стоимостью. Результаты сортируются по убыванию цены. Отмененные заказы не учитываются.

    [![image](https://github.com/user-attachments/assets/9ce3f9fd-f802-4b25-a6ec-23647404a1ae)
фото 5]

2.  **Два самых дорогих заказа:** Нужно получить два заказа с максимальной стоимостью. Данные сортируются по убыванию цены, отмененные заказы исключаются.

    [![image](https://github.com/user-attachments/assets/e868f613-f85c-4e88-bac9-c2f00a31f8ad)
 фото 6]

3.  **Добавление нового заказа:** В таблицу `orders` добавляется информация о новом заказе на сумму 8000 рублей, состоящем из 4 товаров (`products`).

    [![image](https://github.com/user-attachments/assets/e1bbc4a2-46ce-40fc-8d82-4aa9ebeb0d5c)
фото 7]
    [![image](https://github.com/user-attachments/assets/550055a6-e9ea-4ab5-a596-0d5c9289d118)
![image](https://github.com/user-attachments/assets/76a5694a-098b-499d-a88a-4814499abe8c)
фото 8]

4.  **Добавление нового товара:** В таблицу `products` вносятся данные о новом товаре: "VR-очки" стоимостью 70000 рублей, в количестве 2 штук (`count`).

    [![image](https://github.com/user-attachments/assets/21016e68-42fb-425c-b37f-52179daae3b7)
фото 9]
    [![image](https://github.com/user-attachments/assets/80ae7fa7-457e-4267-a83c-0c1a09c4e9d7)
фото 10]

5.  **Исправление ошибки в названии товара:** В таблице `products` название товара "IMAC" исправляется на "PS5".

    [![image](https://github.com/user-attachments/assets/89ff3aac-0287-4c9a-a367-d1b37ed19034)
фото 11]
    [![image](https://github.com/user-attachments/assets/0aaf3715-c88a-421b-8581-bd16e17c4444)
фото 12]

**Полезные команды (шпаргалки)**

*   **Вставка одной строки:** `INSERT INTO table (column1, column2) VALUES (value1, value2);` (Добавление новой строки в таблицу с указанием значений для заданных столбцов).
*   **Вставка нескольких строк:** `INSERT INTO table (column1, column2) VALUES (value11, value12), (value21, value22), ...` (Добавление нескольких строк одновременно).
*   **Копирование данных из другой таблицы:** `INSERT INTO table1 (column1, column2) SELECT (col1, col2) FROM table2;` (Перенос данных из одной таблицы в другую).
*   **Изменение данных во всех строках:** `UPDATE table1 SET column1 = new value;` (Обновление значения указанного столбца во всех строках таблицы).
*   **Изменение данных по условию:** `UPDATE table1 SET column1=new_value, column2=new_value WHERE condition;` (Обновление значений столбцов только в тех строках, которые соответствуют условию).
*   **Удаление всех строк:** `DELETE FROM table;` (Полная очистка таблицы).
*   **Удаление строк по условию:** `DELETE FROM table WHERE condition;` (Удаление строк, соответствующих заданному условию).
