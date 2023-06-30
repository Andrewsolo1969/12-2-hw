# 12-2-hw

# Домашнее задание к занятию "11.2 «Кеширование Redis/memcached»" - Соловьёв Андрей SYS-18

---

Работа была выполнена на виртуальной машине с Linux Mint, организованной с помощью Oracle VM VirtualBox.



## Задание 1. Кеширование

Приведите примеры проблем, которые может решить кеширование.Приведите примеры проблем, которые может решить кеширование.


Из материалов презентации:

- Повышение производительности за счет складывания в кэш данных, к которым чаще всего происходит обращение;

- Увеличение скорости ответа;

- Экономия ресурсов базы данных, например, применяя кэширование тяжелых запросов;

- Сглаживание бустов трафика, чтобы переживать резкое увеличение (скачки) трафика.



## Задание 2. Memcached

Установите и запустите memcached.

Приведите скриншот systemctl status memcached, где будет видно, что memcached запущен.


memcached установлен  -  apt install memcached

и запущен - systemctl status memcached

![memcached started.png](https://github.com/Andrewsolo1969/11-2-hw/blob/master/img/memcached_started.PNG)


## Задание 3. Удаление по TTL в Memcached

Запишите в memcached несколько ключей с любыми именами и значениями, для которых выставлен TTL 5.

Приведите скриншот, на котором видно, что спустя 5 секунд ключи удалились из базы.

Ключ с TTL 20 - видно, что ключ в базе ещё присутствует.


![key_ttl_20](https://github.com/Andrewsolo1969/11-2-hw/blob/master/img/key_ttl_20.PNG)


Ключ с TTL 5 - видно, что ключ удалился из базы.


![key_ttl_5](https://github.com/Andrewsolo1969/11-2-hw/blob/master/img/key_ttl_5.PNG)



## Задание 4. Запись данных в Redis

Запишите в Redis несколько ключей с любыми именами и значениями.

Через redis-cli достаньте все записанные ключи и значения из базы, приведите скриншот этой операции.

Redis установлен 


![Redis_installed](https://github.com/Andrewsolo1969/11-2-hw/blob/master/img/Redis_installed.PNG)


и запущен


![Redis_started](https://github.com/Andrewsolo1969/11-2-hw/blob/master/img/Redis_started.PNG)


Redis_cli

![redis_cli](https://github.com/Andrewsolo1969/11-2-hw/blob/master/img/redis_cli.PNG)


Запись ключей через redis-cli и поиск ключей в хранилище данных.

![Redis_keys](https://github.com/Andrewsolo1969/11-2-hw/blob/master/img/Redis_keys.PNG)












 
