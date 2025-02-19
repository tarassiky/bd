# bd

# Лабораторная работа №1

# Задание 1

Раздел "Management":

1.Раздел "Server Status":
- Общая информация: название хоста, номер порта, версия БД.
- Настройки сервера: статус брандмауэра, использование SSL.
- Каталоги сервера.
- Сводка по ресурсам: ОЗУ, процессор и т.д.
- Настройки SSL (если включено).

2.Раздел "Client Connections":
- Сведения о подключениях: идентификатор процесса, тип, пользователь, хост, дополнительная информация.
- Блокировки: информация о блокировках.
- Атрибуты подключения: ОС, имя клиента, версия клиента, платформа.

3.Раздел "Users and Privileges":
- Управление учетными записями: кнопки "Add Account", "Delete", "Refresh".
- Информация о выбранной учетной записи: имя логина, тип аутентификации, ограничения на хосты, пароль.
- Ограничения учетной записи: количество запросов, обновлений, подключений.
- Роли: быстрый способ предоставления привилегий.
- Привилегии схем: назначение прав доступа к схемам.

4.Раздел "Status and Systems Variables":
- Список серверных переменных для активного подключения.
- Установка глобальных системных переменных.

5.Разделы "Data Export" и "Data Import":
- Мастер экспорта и импорта табличных данных: CSV, JSON, параметры конфигурации.
- Мастер экспорта и импорта данных SQL: использование mysqldump.
- Экспорт и импорт данных результатов.


Раздел "Instance":

1.Раздел "Startup/Shutdown":
- Просмотр журнала сообщений о запуске.
- Запуск и завершение работы экземпляра MySQL.
- Просмотр текущего состояния экземпляра.

2.Раздел "Server Logs":
- Отображение информации журнала для сервера MySQL.
- Вкладки для общих журналов ошибок и журналов замедления.

3.Раздел "Options File":
- Просмотр и редактирование файла конфигурации MySQL.
- Группировка опций, поле поиска, путь к файлу конфигурации.


Раздел "Performance":

1.Раздел "Dashboard":
- Статистика сетевого трафика, клиентских подключений.
- Основная активность сервера MySQL и статистика производительности.
- Обзор InnoDB Buffer Pool и активности диска.

2.Раздел "Performance Reports":
- Графический интерфейс для настройки и тонкой настройки схемы производительности.

3.Раздел "Performance Schema Setup":
- Отчеты на основе схемы производительности для анализа работы сервера MySQL.
- Анализ горячих точек ввода-вывода, дорогостоящих инструкций SQL, статистики ожидания и показателей InnoDB.


![image](https://github.com/user-attachments/assets/63c7afc9-dd63-432e-8f68-c63c0fbfce92)

# Задание 2

![image](https://github.com/user-attachments/assets/6b92b84e-d8b6-4d5d-ab01-fb349b63bec8)
![image](https://github.com/user-attachments/assets/b23bd433-fdfa-4493-9c8d-ab0895e37f8a)

# Задание 3

![image](https://github.com/user-attachments/assets/d10ebf08-3f90-4edb-b01d-6f9eb0b3049f)

# Задание 4

CREATE TABLE `users` (
  `id` int NOT NULL AUTO_INCREMENT,
  `name` varchar(45) NOT NULL,
  `email` varchar(45) NOT NULL,
  PRIMARY KEY (`id`),
  UNIQUE KEY `email_UNIQUE` (`email`)
) ENGINE=InnoDB AUTO_INCREMENT=4 DEFAULT CHARSET=utf8mb3;

![image](https://github.com/user-attachments/assets/943cbc43-a174-4595-bba8-168f4140fd37)

![image](https://github.com/user-attachments/assets/ea99be3d-759d-4a3c-9b6e-d7d99ac4bcff)   ![image](https://github.com/user-attachments/assets/3e0fd301-32c8-44dc-a898-993277d35e39)

# Задание 5

![image](https://github.com/user-attachments/assets/ceccc0ce-e561-4363-ab60-98e4be5c6793)   ![image](https://github.com/user-attachments/assets/e18c2ca6-147c-42eb-84d5-eb1b57a6e3fe)

CURRENT_TIMESTAMP возвращает текущую дату и время в часовом поясе сеанса в значении типа данных TIMESTAMP (Хранит значение даты и времени в виде ГГГГ-MM-ДД ЧЧ:ММ:СС. От 1970-01-01 00:00:01 до 2038-01-19 03:14:07) c указанием часового пояса

Поля, которые могут быть NULL:
name: Пользователь может не захотеть указывать своё имя.
email: Электронная почта также может оставаться необязательной для заполнения.
gender: Пол тоже является личной информацией, которую пользователь может предпочесть скрыть.
bday: Дата рождения – ещё одно поле, которое многие люди предпочитают оставлять незаполненным.
postal_code: Почтовый индекс может не указываться пользователем, особенно если он не связан с доставкой товаров или услуг.
rating: Рейтинг может отсутствовать до тех пор, пока система не начнёт его вычислять, поэтому это поле также может быть NULL.

Поля, которые должны быть NOT NULL:
id: Идентификатор записи всегда должен быть уникальным и ненулевым.
created: Время создания записи должно фиксироваться автоматически при добавлении новой строки, так что оно не может быть NULL.

# Задание 6

![image](https://github.com/user-attachments/assets/bb08f63b-613f-46a3-8384-1cbbc254ede1)

![image](https://github.com/user-attachments/assets/78cb0afd-14c6-401a-b166-18e2c61d6c3a)   ![image](https://github.com/user-attachments/assets/92aa5c4b-fb4a-470b-9a87-427934f1a935)

# Задание 7

![image](https://github.com/user-attachments/assets/23f06669-fce3-4299-9d3c-110dfaef13dc)

Между знаками “/*…*/” указана информация, из какой базы данных была взята информация, а также дата экспорта в данный файл.
Далее указаны заполненные поля таким образом, что после INSERT INTO указаны атрибуты, а после VALUES указаны наполняемое, соответствующее указанным атрибутам; на каждой новой строке указывается новая строка для самой таблицы.

# Задание 8

![image](https://github.com/user-attachments/assets/c2b3fe6e-0904-49bd-8dda-ab1b4eb7660f)

![image](https://github.com/user-attachments/assets/c132ac3a-c0ad-44fc-bea9-988a5eb9fe27)   ![image](https://github.com/user-attachments/assets/4cf0ab23-a0b5-4d92-b63f-2319a45a2e30)

CREATE TABLE `resume` (
  `resumeid` int NOT NULL AUTO_INCREMENT,
  `userid` int NOT NULL,
  `title` varchar(100) NOT NULL,
  `skills` text,
  `created` timestamp NULL DEFAULT CURRENT_TIMESTAMP,
  PRIMARY KEY (`resumeid`),
  KEY `userid_idx` (`userid`),
  CONSTRAINT `userid` FOREIGN KEY (`userid`) REFERENCES `users` (`id`) ON DELETE CASCADE ON UPDATE CASCADE
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb3;

В данном SQL-запросе выполняется создание таблицы с некоторыми параметрами. Также указывается первичный ключ ‘resumeid’ и внешний ключ ‘userid’, который ссылается на таблицу “users”, атрибуту ‘id’. 
Указаны параметр CASCADE при удалении или обновлении, что означает, что при выполнении данных действий в родительской таблице изменения автоматически произведутся в дочерних таблицах

![image](https://github.com/user-attachments/assets/2271f9d2-0c3d-452b-af0f-b8bb528c0b32)   ![image](https://github.com/user-attachments/assets/eae6a200-db93-4587-afeb-93988253b79e)

# Задание 9

![image](https://github.com/user-attachments/assets/04e09454-1270-49b2-a14c-7d46e78989bd)   ![image](https://github.com/user-attachments/assets/36ac180f-61b7-4e21-9600-969a128694cb)

![image](https://github.com/user-attachments/assets/04d6700a-cd6a-4f99-8f24-fb9d7ff81ca5)

Минимальное количество резюме у одного пользователя - ноль
Максимальное количество резюме у одного пользователя может быть неограниченно 

![image](https://github.com/user-attachments/assets/b82f8620-3bb0-4e53-b95a-2fd6af3abba9)

![image](https://github.com/user-attachments/assets/a99145f5-b2dd-4ad9-92dd-e7712b409c02)

При попытке описания строки с несуществующем в “users” ‘id’ программа выдает ошибку.

Таким образом мы получили еще одну таблицу, в которой есть несколько данных о персонажах из прошлой таблицы. Кроме того, экспериментально выяснили, что добавить информацию во вторую таблицу о людях, неотмеченных в первой таблице невозможно.

# Задание 10

![image](https://github.com/user-attachments/assets/9c601a7b-c9e7-48ac-89a0-fd7af089b3d7)   ![image](https://github.com/user-attachments/assets/29ac3252-14f2-4996-917f-d335f71def25)

![image](https://github.com/user-attachments/assets/43569f3e-8c8d-4cb9-a737-aa0f08aca31c)

При удалении пользователя Madaline из таблицы “users” удаляются его резюме (строки) в таблице резюме.

![image](https://github.com/user-attachments/assets/30afcbd1-3f3a-4de0-bef3-ce2a60f9b29a)   ![image](https://github.com/user-attachments/assets/99a401ff-a217-4f21-84c3-e0e17a29c41e)

При изменении ‘id’ в таблице “users” изменяет ‘id’ в таблице резюме
