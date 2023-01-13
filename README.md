# OZON
## Оглавление
1. [Описание проекта](#описание-проекта)
2. [Майнд-карта](#майнд-карта)
3. [Чек-листы](#чек-листы)  
          1. [Пример чек-листа с применением техник КЭ и ГЗ](#пример-чек-листа-с-применением-техник-кэ-и-гз)  
          2. [Примеры чек-листов с применением техники предугадывания ошибок](#примеры-чек-листов-с-применением-техники-предугадывания-ошибок)  
4. [Тест-кейсы](#тест-кейсы)     
5. [Прочие техники тест-дизайна и методы тестирования](#прочие-техники-тест-дизайна-и-методы-тестирования)      
          1.[Тестирование с помощью таблицы решений](#тестирование-с-помощью-таблицы-решений)    
          2.[Тестирование состояний и переходов](#тестирование-состояний-и-переходов)     
          3.[Попарное тестирование](#попарное-тестирование)    
          4.[Тест-сессия](#тест-сессия)    
          5.[Тест-туры](#тест-туры)     
6. [Баг-репорты](#баг-репорты) 
7. [План тестирования исправления багов](#план-тестирования-исправления-багов)
8. [Команды MySQL](#команды-mysql)
9. [Тестирование API](#тестирование-api)
## Описание проекта
Здесь представлены планы, процессы и результаты тестирования сайта https://www.ozon.ru, а также другие практические навыки, которые я применяла в рамках курса. 
## Майнд-карта
Данная майнд-карта представляет собой набор тестов для тестирования объекта **Товары**. Подробная проверка расписана для компонентов **Поиск товара** и **Покупка**.
<img width="1963" alt="Товар" src="https://user-images.githubusercontent.com/122577498/212377271-994ac3c2-c672-4c30-b53a-26727bd32de9.png">
## Чек-листы
### Пример чек-листа с применением техник КЭ и ГЗ
Для тестирования взят объект **Поиск**.

<img width="639" alt="Снимок экрана 2023-01-13 в 20 14 58" src="https://user-images.githubusercontent.com/122577498/212380159-ef2e1893-5fa5-4246-a99a-92ac4e0fa1d3.png">

---------------------

### Примеры чек-листов с применением техники предугадывания ошибок
Для тестирования использовались объекты **Товары**, **Заказ** и **Возврат**.

<img width="506" alt="Снимок экрана 2023-01-13 в 20 23 53" src="https://user-images.githubusercontent.com/122577498/212381558-bb476016-a050-4346-9fe3-3f6972b22bfe.png">

## Тест-кейсы
Здесь представлены примеры тест-кейсов, созданных на платформе **TestLink**. Для тестирования взят объект **Авторизация**.

<img width="836" alt="Снимок экрана 2023-01-13 в 20 38 54" src="https://user-images.githubusercontent.com/122577498/212385692-1b442da3-4ad1-45f7-8a3d-a7f43de3d204.png">

----------------------

<img width="847" alt="Снимок экрана 2023-01-13 в 20 39 51" src="https://user-images.githubusercontent.com/122577498/212385750-2ddc0534-07a0-4070-a791-dcc52ab17f14.png">

## Прочие техники тест-дизайна и методы тестирования
### Тестирование с помощью таблицы решений
Здесь представлен пример таблицы решений. В качестве объекта тестирования рассматривается акция **"Баллы за отзывы"**.

<img width="809" alt="Снимок экрана 2023-01-13 в 21 25 20" src="https://user-images.githubusercontent.com/122577498/212392523-76d72ee7-aa90-4a46-ba21-3fa312a4c3e9.png">

----------------------

### Тестирование состояний и переходов
Пример диаграммы и таблицы состояний и переходов для объекта **Заказ**, а также чек-лист на основании сделанной таблицы.
#### Диаграмма

<img width="570" alt="Снимок экрана 2023-01-13 в 21 38 36" src="https://user-images.githubusercontent.com/122577498/212394603-ab69534e-c9c9-41d8-8219-e042050290ae.png">

#### Таблица состояний и переходов

<img width="1191" alt="Снимок экрана 2023-01-13 в 21 41 11" src="https://user-images.githubusercontent.com/122577498/212395029-a662da5d-3868-48b6-b0c1-587fa055dedc.png">

#### Чек-лист на основании таблицы

<img width="497" alt="Снимок экрана 2023-01-13 в 21 43 47" src="https://user-images.githubusercontent.com/122577498/212395501-5d4df045-7271-4525-941b-1c996b8ac2ff.png">

------------------------------

### Попарное тестирование
Данная техника использовалась для тестирования фичи **Поиск авиабилетов OZON**. Применялся генератор таблиц https://pairwise.teremokgames.com.

<img width="921" alt="Снимок экрана 2023-01-13 в 21 51 29" src="https://user-images.githubusercontent.com/122577498/212396837-e75334d6-ab3f-47f5-8353-237a21577358.png">

--------------------------------

### Тест-сессия
Здесь представлен пример тест-сессии для объекта **Поиск товара** и отчет по проведенной сессии.

##### Цель:
Проверить поиск товара через каталог и через поисковую строку, проверить атрибуты поиска, включая работу фильтров и заданных параметров, а так же соответствие найденного товара установленным значениям.
##### Функционал:
###### 1.Поисковая строка
а) Поиск товаров по разным наименованиям, цифрам, символам

б) Поиск товаров по имеющимся категориям
###### 2. Каталог
а) Поиск товаров через меню "Каталог"
###### 3. Фильтры и параметры
а) проверить работу фильтров и заданных параметров

б) проверить соответствие найденного товара указанным значениям

<img width="826" alt="Снимок экрана 2023-01-13 в 22 02 59" src="https://user-images.githubusercontent.com/122577498/212398608-5eea55ac-bbdc-4e95-8203-3b7ecfb739d4.png">

------------------------------

### Тест-туры
В этом разделе перечислены основные тест-туры, которые, на мой взгляд, лучше всего подходят для тестирования сайта **OZON**, а также тест-тур, придуманный лично мной. К каждому тест-туру добавлено небольшое описание.
- ##### Тур супермодели 
Раз главная функция сайта – продажа товаров, то и сам сайт должен выглядеть продаваемо, с годным визуалом, удачными фотографиями самих товаров, понятной навигацией и тд.
- ##### Тур лежебоки 
На сайте много функций для ленивых: "экспресс доставка", "купить в один клик" и тд, плюс пользователи часто заходят с целью быстро купить нужное, им лень заполнять поля и нажимать на дополнительные кнопки.
- ##### Антиобщественный тур
Надо посмотреть, не продаются ли случайно на сайте продукты, запрещенные к продаже, нельзя ли дважды оформить возврат и тд.
- ##### Денежный тур
Так как основная функция - продавать товары, надо проверить весь функционал, связанный с финансами, оплатой, возвратами и тд, чтобы из-за багов сайт не нес убытки.
- ##### Тур коллекционера 
Исследовать все кнопки (озон бизнес, билеты, отели, акции, горячее кнопки и тд). То, на что постоянные пользователи особо внимания не обращают.
- ##### Тур нервного покупателя
Разработан мной с учетом специфики сайта и возможного поведения пользователей. Мы не просто оформляем заказ, а двести раз удаляем-добавляем товар, меняем количество, отменяем, заказываем снова, делаем возврат и пишем сообщения в поддержку. То есть одновременно и пытаемся поломать ПО, и охватываем разный функционал сразу.

## Баг-репорты
Здесь представлены примеры оформленных баг-репортов с локализацией ошибок. Для оформления использовался баг-трекер **Redmine**.

<img width="708" alt="Снимок экрана 2023-01-13 в 22 31 30" src="https://user-images.githubusercontent.com/122577498/212405047-890db411-4bc0-4038-848f-37c5b9ee7ae7.png">

------------------------------------------

<img width="1193" alt="Снимок экрана 2023-01-13 в 22 39 52" src="https://user-images.githubusercontent.com/122577498/212405169-01be7cc2-b951-4a27-b0f2-d635193e4ec1.png">

## План тестирования исправления багов
Здесь представлен план подтверждающего и регрессионного тестирования исправления багов на примере двух найденных багов.

<img width="901" alt="Снимок экрана 2023-01-13 в 22 48 08" src="https://user-images.githubusercontent.com/122577498/212406215-918337b3-f7cc-4959-aa86-91a3633e9de1.png">

## Команды MySQL
Здесь представлена работа с БД на примере программы **MySQL** и основные запросы для БД **shop**, таблицы **goods**.
##### Создание БД
```javascript
CREATE SCHEMA `shop` DEFAULT CHARACTER SET utf8 COLLATE utf8_bin ;
```
##### Создание таблицы из двух столбцов
```javascript
CREATE TABLE `shop`.`goods` (
`id` INT NOT NULL AUTO_INCREMENT,
`name` VARCHAR(45) NOT NULL,
PRIMARY KEY (`id`));
```
##### Добавление нового столбца
```javascript
ALTER TABLE `shop`.`goods`
ADD COLUMN `size` INT NOT NULL AFTER `name`;
```
##### Добавление значений в таблицу
```javascript
INSERT INTO goods (`name`, `size`) VALUES ('очки солнцезащитные', '5');
```
##### Поменять значения в таблице
```javascript
UPDATE goods SET size = 2 WHERE id = 1;
```
##### Удалить значения в таблице
```javascript
DELETE FROM goods WHERE id = 5;
```
##### Удалить таблицу
```javascript
DROP TABLE `shop`.`goods`;
```
##### Комбинированные запросы
```javascript
SELECT * FROM goods WHERE id < 4 LIMIT 2;
SELECT * FROM goods WHERE size > 1 ORDER BY size DESC;
```
## Тестирование API
В этом разделе представлены запросы, использованные для методов **POST**, **GET**, **PUT** и **DELETE**, а также примеры тестов для методов **PUT** и **DELETE**. В качестве проекта взят тестовый сайт https://dummyapi.io.
### POST (Сreate User)
Создает нового пользователя и возвращает данные о нем.
#### Request Body
```json
{
"title": "ms",
"firstName": "Eva",
"lastName": "Bombina",
"gender": "female",
"email": "ebombina@yandex.ru",
"dateOfBirth": "9/4/1994",
"phone": "8921xxxxxxx",
"picture": "http://myphoto.com",
"location": 
     {
"street": "Prazhskaya",
"city": "St Petersburg",
"state": "No",
"country": "Russia",
"timezone": "+7:00"
     }
}
```
#### Response Body
```json
{
    "id": "63b4d4cecef326a4129a62cc",
    "title": "ms",
    "firstName": "Eva",
    "lastName": "Bombina",
    "picture": "http://myphoto.com",
    "gender": "female",
    "email": "ebombina@yandex.ru",
    "dateOfBirth": "1994-09-04T00:00:00.000Z",
    "phone": "8921xxxxxxx",
    "location": {
        "street": "Prazhskaya",
        "city": "St Petersburg",
        "state": "No",
        "country": "Russia",
        "timezone": "+7:00"
    },
    "registerDate": "2023-01-04T01:22:22.592Z",
    "updatedDate": "2023-01-04T01:22:22.592Z"
}
```
----------------------------
### GET (Get List)
Возвращает список пользователей. В данном запросе установлен лимит на 10 первых пользователей.

<img width="1010" alt="Снимок экрана 2023-01-05 в 01 16 51" src="https://user-images.githubusercontent.com/122577498/212420787-3111d9f5-3eef-4e34-9b3b-ed746ae4b139.png">

-----------------------------

### PUT (Update User)
Вносит изменения в информацию о пользователе, возвращает обновленные данные. В представленном запросе меняется часовой пояс.

<img width="1009" alt="Снимок экрана 2023-01-05 в 01 26 02" src="https://user-images.githubusercontent.com/122577498/212421914-77956321-2458-4b18-b635-82076e8bb816.png">

------------------------------

### DELETE (Delete User)
Удаляет пользователя, возвращает id удаленного пользователя.

<img width="1011" alt="Снимок экрана 2023-01-05 в 01 31 33" src="https://user-images.githubusercontent.com/122577498/212422601-5e5c8ab4-32e9-4160-b56c-be7da22c1855.png">

----------------------------

### Пример проверок для метода **PUT**
- Ввести некорректный id пользователя
- Ввести id другого пользователя
- Попробовать исправить email 
### Пример проверок для метода **DELETE**
- Удалить пользователя с несуществующим id
- Удалить другого пользователя
- Удалить пользователя и попробовать найти его по идентификатору












