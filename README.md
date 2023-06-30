
# Домашнее задание к занятию "12.2 «Работа с данными (DDL/DML)»" - Соловьёв Андрей SYS-18

---

Работа была выполнена на виртуальной машине с Linux Lite 6.4


## Задание 1


1.1. Поднимите чистый инстанс MySQL версии 8.0+. Можно использовать локальный сервер или контейнер Docker.

![mysql_active.png](https://github.com/Andrewsolo1969/12-2-hw/blob/main/img/mysql_active.png)

1.2. Создайте учётную запись sys_temp.

![sys_temp_created.png](https://github.com/Andrewsolo1969/12-2-hw/blob/main//img/sys_temp_created.png)

1.3. Выполните запрос на получение списка пользователей в базе данных. (скриншот)

![user_list.png](https://github.com/Andrewsolo1969/12-2-hw/blob/main//img/user_list.png)

1.4. Дайте все права для пользователя sys_temp.

![PRIVILEGES.png](https://github.com/Andrewsolo1969/12-2-hw/blob/main//img/PRIVILEGES.png)

1.5. Выполните запрос на получение списка прав для пользователя sys_temp. (скриншот)

![show_priv.png](https://github.com/Andrewsolo1969/12-2-hw/blob/main//img/show_priv.png)

1.6. Переподключитесь к базе данных от имени sys_temp.

ALTER USER 'sys_temp'@'localhost' IDENTIFIED WITH mysql_native_password BY '1111';

![alter_user.png](https://github.com/Andrewsolo1969/12-2-hw/blob/main//img/alter_user.png)

1.6-7 По ссылке https://downloads.mysql.com/docs/sakila-db.zip скачал дамп базы данных и Восстановил дамп в базу данных.Sakila

![restore.png](https://github.com/Andrewsolo1969/12-2-hw/blob/main//img/restore.png)

![FULL_TABLES.png](https://github.com/Andrewsolo1969/12-2-hw/blob/main//img/FULL_TABLES.png)


1.8. При работе в IDE сформируйте ER-диаграмму получившейся базы данных. При работе в командной строке используйте команду для получения всех таблиц базы данных. (скриншот)

![diagram.png](https://github.com/Andrewsolo1969/12-2-hw/blob/main//img/diagram.png)

![TABLES.png](https://github.com/Andrewsolo1969/12-2-hw/blob/main//img/TABLES.png)


## Задание 2

Составьте таблицу, используя любой текстовый редактор или Excel, в которой должно быть два столбца: в первом должны быть названия таблиц восстановленной базы, во втором названия первичных ключей этих таблиц. Пример: (скриншот/текст)

Название таблицы | Название первичного ключа
customer         | customer_id


![Table_id.png](https://github.com/Andrewsolo1969/12-2-hw/blob/main//img/Table_id.png)


