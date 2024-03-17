# Домашнее задание к занятию  «Защита хоста - Тихун Вадим SYS-25»

------

### Задание 1

1. Установите **eCryptfs**.
2. Добавьте пользователя user2.
3. Зашифруйте домашний каталог пользователя с помощью eCryptfs.


*В качестве ответа  пришлите снимки экрана домашнего каталога пользователя с исходными и зашифрованными данными.*  

### Ответ 1

1. Установил **eCryptfs**


![1install](https://github.com/sailent9/sdb-homeworks/assets/130309754/52d10951-eeea-47ab-b510-a600ad6f3a6f)

2. Добавил пользвателя c шифрованием домашнего каталога **user2**


![2adduser](https://github.com/sailent9/sdb-homeworks/assets/130309754/50f8fb5e-0abf-4cd5-a3f5-7395ff2a2758)

- переключился на пользователя `user2` и создал простой файл `123,456`


![3user2](https://github.com/sailent9/sdb-homeworks/assets/130309754/aa66c5de-cee8-40b6-bf8c-f640865a9b31)

- посмотрел утилитой `ls -la`
- зашел под пользователем `abc` и проверил доступность домашнего каталога `user2`

3. Ответ системы из под другого пользователя:


-![4ls-la](https://github.com/sailent9/sdb-homeworks/assets/130309754/576c5f5d-a807-43cf-bce6-7679a7676eab)
--





### Задание 2

1. Установите поддержку **LUKS**.
2. Создайте небольшой раздел, например, 100 Мб.
3. Зашифруйте созданный раздел с помощью LUKS.

*В качестве ответа пришлите снимки экрана с поэтапным выполнением задания.*

### Ответ 2

1. Устанавливаю `Luks`:


![1instluks](https://github.com/sailent9/sdb-homeworks/assets/130309754/a02cdc4c-b46e-4a56-8549-7e87679e89a5)

2. Далее необходимо выделить место под диск. Запускаю ВМ в Live CD режиме, потом отмонтировал основной диск и уменьшил его размер с помощью      `Gparted` на 100 Мб, для последующей работы с этим разделом.
![2resize](https://github.com/sailent9/sdb-homeworks/assets/130309754/4305dfb0-d207-4958-9815-0f7f9e8137c9)
![3resizefin](https://github.com/sailent9/sdb-homeworks/assets/130309754/099ab2fc-ab20-45ed-bd12-ca9e31ed34db)
![4appling](https://github.com/sailent9/sdb-homeworks/assets/130309754/f8b6a345-d8b4-42df-8bde-d9c195d4a5d9)
![5sda4](https://github.com/sailent9/sdb-homeworks/assets/130309754/a8141194-9584-4a1b-b564-a94198adeaf8)


3. Далее форматирую этот раздел:(При согласии обязательно указать заглавными буквами полное слово: YES)


![6luksformat](https://github.com/sailent9/sdb-homeworks/assets/130309754/3773fe30-145e-4e36-b77e-5f7424bb0a3b)

4. Монтирую этот раздел:


![7luksOpen](https://github.com/sailent9/sdb-homeworks/assets/130309754/3405a254-9cf9-4ea4-bd77-28f62b455fe7)

5. Форматирую диск:


![8form](https://github.com/sailent9/sdb-homeworks/assets/130309754/384490de-cebf-4a81-90ed-5acafefa6c47)

6. Создаю скрытую деркторию и монтирую к ней диск:


![9mount](https://github.com/sailent9/sdb-homeworks/assets/130309754/0eb84ef4-fe09-4cab-8078-ff7adda12ea1)

---
