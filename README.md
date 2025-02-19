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

![1](https://github.com/user-attachments/assets/c72e20cb-a2d6-438a-b94f-ffb9d7ca8fbb)

# Задание 2

![2](https://github.com/user-attachments/assets/ed8c82e1-a6dd-4d44-813a-5647d57c6ade)
![3](https://github.com/user-attachments/assets/728ac974-b383-48e6-a4ac-f50a1a9b79e3)

# Задание 3

![4](https://github.com/user-attachments/assets/bcd6635a-bc0f-4ebd-bb43-22d6442a3e1b)


# Задание 4

CREATE TABLE `users` (
  `id` int NOT NULL AUTO_INCREMENT,
  `name` varchar(45) NOT NULL,
  `email` varchar(45) NOT NULL,
  PRIMARY KEY (`id`),
  UNIQUE KEY `email_UNIQUE` (`email`)
) ENGINE=InnoDB AUTO_INCREMENT=4 DEFAULT CHARSET=utf8mb3;

![5](https://github.com/user-attachments/assets/06f8dc39-0648-4719-8631-53aa111eb9a4)

![6](https://github.com/user-attachments/assets/76384d7e-f8c8-4fba-afee-1f83db94d7a6)  ![7](https://github.com/user-attachments/assets/e50a1b90-04bc-4c18-a3aa-b6de85b736c1)

# Задание 5

![8](https://github.com/user-attachments/assets/42edda95-60e5-4c93-9ba5-f91e4735970d)  ![9](https://github.com/user-attachments/assets/8d0e43fd-96db-4884-b907-70cb374a08d4)

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

![10](https://github.com/user-attachments/assets/2411e5f9-a004-4734-9fc0-0beada43325e)

![11](https://github.com/user-attachments/assets/849ce760-69fd-470b-9907-b7e7eb0efecf)   ![12](https://github.com/user-attachments/assets/d09df668-d411-48a2-bf92-cf40f20a0435)

# Задание 7

![13](https://github.com/user-attachments/assets/2a1b097b-ab84-4818-94cd-2526a67756fb)

Между знаками “/*…*/” указана информация, из какой базы данных была взята информация, а также дата экспорта в данный файл.
Далее указаны заполненные поля таким образом, что после INSERT INTO указаны атрибуты, а после VALUES указаны наполняемое, соответствующее указанным атрибутам; на каждой новой строке указывается новая строка для самой таблицы.

# Задание 8

![14](https://github.com/user-attachments/assets/8c3645bf-aa6c-41c5-9793-9a5fcf11298c)

![15](https://github.com/user-attachments/assets/557c4b9d-965e-4463-918a-e844c6eb768e)   ![16](https://github.com/user-attachments/assets/793906ba-d852-4e43-8f0f-407828a8fade)

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

![17](https://github.com/user-attachments/assets/7fbbb883-728a-48a6-b534-8f32926dcbaa)   ![18](https://github.com/user-attachments/assets/f47bd0ed-18ec-4a4c-ae7a-7742001c4e9b)

# Задание 9

![19](https://github.com/user-attachments/assets/4defab36-3a43-461e-9b85-0eb9c855735f)   ![20](https://github.com/user-attachments/assets/4ae5422b-6a2d-46a1-a020-0c3ae9de1bb1)

![21](https://github.com/user-attachments/assets/8fedaf0f-6aa8-4088-b3bd-5ad0b73c52de)

Минимальное количество резюме у одного пользователя - ноль
Максимальное количество резюме у одного пользователя может быть неограниченно 

![22](https://github.com/user-attachments/assets/6e2e61c7-ba8a-4b13-95c6-cdec9d83f03c)

![23](https://github.com/user-attachments/assets/6954980f-e665-4e7e-b9cc-54a10fe5aad9)

При попытке описания строки с несуществующем в “users” ‘id’ программа выдает ошибку.

Таким образом мы получили еще одну таблицу, в которой есть несколько данных о персонажах из прошлой таблицы. Кроме того, экспериментально выяснили, что добавить информацию во вторую таблицу о людях, неотмеченных в первой таблице невозможно.

# Задание 10

![24](https://github.com/user-attachments/assets/7b9f7300-9c65-433f-a8c3-de4e93887afd)   ![25](https://github.com/user-attachments/assets/e8f37baa-632b-42b9-849e-1892dc27955d)

![26](https://github.com/user-attachments/assets/6e9e8a27-c69d-4203-b77d-ff18f56449b8)

При удалении пользователя Madaline из таблицы “users” удаляются его резюме (строки) в таблице резюме.

![27](https://github.com/user-attachments/assets/b3e313ae-0012-4a53-8a64-0fd0d860bb10)   ![28](https://github.com/user-attachments/assets/240cdd24-4420-447d-945f-70efee3b6d68)

При изменении ‘id’ в таблице “users” изменяет ‘id’ в таблице резюме
