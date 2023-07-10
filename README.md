- [Документация и API](#документация-и-api)
- [Начало работы](#начало-работы)
  - [Регистрация](#регистрация)
  - [Регистрация физ. лица](#регистрация-физ-лица)
  - [Добавление магазина](#добавление-магазина)
  - [Настройка магазина](#настройка-магазина)
- [Платежи](#платежи)
  - [Создание платежа](#создание-платежа)
  - [Создание простой формы в личном кабинете](#создание-простой-формы-в-личном-кабинете)
  - [Передача информации о заказе](#передача-информации-о-заказе)
  - [Уведомление об оплате](#уведомление-об-оплате)
- [API](#api)
  - [Общая информация](#общая-информация)
  - [Создание заказа](#создание-заказа)
  - [Список магазинов](#список-магазинов)
  - [Баланс](#баланс)
  - [Проверка заказа](#проверка-заказа)
  - [Список заказов](#список-заказов)
  - [Вывод средств](#вывод-средств)
  - [Список выплат](#список-выплат)
  - [Проверка выплаты](#проверка-выплаты)
- [Справочная информация](#справочная-информация)
  - [Коды платежных систем](#коды-платежных-систем)
  - [Коды моб. телефонов](#коды-моб-телефонов)
  - [Буквенные коды валют](#буквенные-коды-валют)
- [FAQ](#faq)
  - [Тарифы и лимиты](#тарифы-и-лимиты)
  - [Модерация проекта](#модерация-проекта)
  - [Массовые выплаты](#массовые-выплаты)

# Документация и API

API сервиса Tegro.money позволяет принимать платежи, делать возвраты, узнавать статусы операции и многое другое. Для работы по API потребуется магазин в нашей системе.

Здесь вы найдете самую последнюю документацию дляподключения физических и юридических лиц.


# Начало работы

## <a name="register"></a>Регистрация

Tegro.money — это платежный агрегатор для приема оплат на вашем сайте. Система поддерживает различные платежные инструменты в едином пользовательском интерфейсе.

Заполните простую форму регистрации аккаунта на странице https://tegro.money/my/register
![image](https://github.com/aldkfjasdfasdf/tergo_test/assets/134290831/d215b038-9644-4f78-ae52-379dfb118c1e)


## <a name="register_fiz"></a>Регистрация физ. лица

Работа от физического лица ведется через нашего чешского партнера. Вам необходимо только принять условия публичной оферты и иметь мобильный телефон под рукой. Также вы можете зарегистрироваться с помощью аттестата WebMoney. Аттестат при этом должен быть не ниже персонального.


## <a name="add-shop"></a>Добавление магазина
### Добавление магазина
Перейдите на страницу добавления магазина https://tegro.money/my/add-shop/


![image](https://github.com/aldkfjasdfasdf/tergo_test/assets/134290831/5a161a31-46db-4804-8669-35e193fc2a26)

Укажите ссылку на свой магазин, название и описание


![image](https://github.com/aldkfjasdfasdf/tergo_test/assets/134290831/c4e3a13a-8606-4b3a-82c1-c1b366e250c5)

### Основные сведения о проекте

__Название__ проекта используется при совершении платежа в качестве основной информации о названии магазина, в пользу которого мы проводим платеж. Описание проекта поможет быстро определить вашу категорию, а в некоторых случаях понять, за что именно вы планируете принимать платежи.

Название должно соответствовать используемому на сайте наименованию компании, продукта или проекта. В __описании__ необходимо указать вид товаров и / или услуг, которые продаются на сайте.

### Подтверждение

На следующем шаге необходимо подтвердить, что вы являетесь собственником сайта, сделать это можно любым из трех способов

![image](https://github.com/aldkfjasdfasdf/tergo_test/assets/134290831/229d7c7a-48a9-48fc-ae6f-1a7f2c90a8e2)

После подтверждения можно переходить к настройкам сайта


## <a name="settings-shop"></a>Настройка магазина

На странице настроек https://tegro.money/my/shop-settings/ Вы можете внести все необходимые данные для работы Вашего магазина.

В первую очередь нужно сгенерировать либо придумать секретный ключ, который нужен для подписи запросов, а так же указать страницы для перенаправления пользователей и уведомлений

![image](https://github.com/aldkfjasdfasdf/tergo_test/assets/134290831/5a5687ce-f0b6-4a4a-a035-97da606c6e4b)

Теперь можно отправлять проект на модерацию, для этого нажмите на переключатель

![image](https://github.com/aldkfjasdfasdf/tergo_test/assets/134290831/54b299f1-9abc-4b2b-b4c3-adf9f0777045)

После модерации Вам сразу станет доступен прием платежей, не забудьте выбрать нужные платежные системы

![image](https://github.com/aldkfjasdfasdf/tergo_test/assets/134290831/962a7c54-f8ee-4d35-8297-7153883d17ab)

И выбрать кто будет платить комиссию сервиса

![image](https://github.com/aldkfjasdfasdf/tergo_test/assets/134290831/cce3c25c-7947-47ce-a6f9-4d4632ddfcce)

Теперь можно переходить к настройке формы оплаты

# Платежи

## <a name="create-p"></a>Создание платежа

## <a name="create-f"></a>Создание простой формы в личном кабинете

## <a name="info-order"></a>Передача информации о заказе

## <a name="notification-p"></a>Уведомление об оплате

# API

## <a name="all-info"></a>Общая информация

### Получение API ключа

API ключ для доступа к REST сервису Tegro.money можно сгенерировать на странице настроек магазина https://tegro.money/my/shop-settings/

![image](https://github.com/aldkfjasdfasdf/tergo_test/assets/134290831/c99435c5-ed26-4631-9dfe-b486389dd5be)

Все данные в запросах к сервису Tegro.money передаются методом POST по протоколу HTTP на адрес https://tegro.money/api/ *method*. Параметры сообщения упаковываются в JSON-объект.

Вместе с запросом необходимо передавать подпись. Подписывать необходимо тело запроса целиком, в том виде, в котором оно отправляется на сервер Банка (после сериализации тела запроса в JSON для отправки по HTTP).

    В каждом запросе необходимо передавать параметр nonce, отличный от предыдущего! 
    Например, можно использовать текущее время в секундах

Используйте для подписи ваш секретный ключ. Сформируйте подпись с алгоритмом SHA-256.

```
import requests
import json
import hashlib
import hmac
import time

api_key = 'EEFA1913EA9D9351469B1E5D852A'

data = {
    'shop_id': '1913EA9D9351469B1E5D852A',
    'nonce': str(int(time.time()))
}

body = json.dumps(data)
sign = hmac.new(api_key.encode('utf-8'), body.encode('utf-8'), hashlib.sha256).hexdigest()

url = "https://tegro.money/api/orders/"

headers = {
    "Authorization": "Bearer " + sign,
    "Content-Type": "application/json"
}

response = requests.post(url, data=body, headers=headers)
print(response.text)
```

## <a name="create-order"></a>Создание заказа

    POST https://tegro.money/api/createOrder/

Используйте этот метод для получения прямой ссылки на оплату заказа

### Запрос

| Header | type | desc |
|-----------|-----------|-----------|
| Authorization		 | string | Подпись запроса |

| Body | type | desc |
|-----------|-----------|-----------|
shop_id |	string |	Shop ID |
nonce	 |integer	 |Уникальный номер запроса |
currency	 |string |	Валюта оплаты, RUB/USD/EUR etc |
amount |	number |	Сумма оплаты |
order_id |	string |	Номер заказа в Вашем магазине |
payment_system |	integer |	ID платежной системы |
fields |	array |	Данные о покупателе |
receipt |	array |	Данные о корзине |


### Ответ

```
{
  "type": "success",
  "desc": "",
  "data": {
    "id": 755555,
    "url": "https://tegro.money/pay/complete/755555/7f259f856e7682a6e98179036a623696/"
  }
}
```


### Пример запроса

```
{
  "shop_id": "1913EA935149B1E5D852A",
  "nonce": 1613435880,
  "currency": "RUB",
  "amount": 1200,
  "order_id": "test order",
  "payment_system": 5,
  "fields": {
    "email": "user@email.ru",
    "phone": "79111231212"
  },
  "receipt": {
    "items": [
      {
        "name": "test item 1",
        "count": 1,
        "price": 600
      },
      {
        "name": "test item 2",
        "count": 1,
        "price": 600
      }
    ]
  }
}

```

## <a name="shops-list"></a>Список магазинов

    POST https://tegro.money/api/shops/

Получение списка ваших магазинов

### Запрос


| Header | type | desc |
|-----------|-----------|-----------|
| Authorization		 | string | Подпись запроса |

| Body | type | desc |
|-----------|-----------|-----------|
shop_id |	string |	Shop ID |
nonce	 |integer	 |Уникальный номер запроса |

### Ответ

```
{
  "type": "success",
  "desc": "",
  "data": {
    "user_id": 1,
    "shops": [
      {
        "id": 1,
        "date_added": "2020-11-03 18:04:07",
        "name": "DEMO1",
        "url": "https://demo1",
        "status": 1,
        "public_key": "D0F98E7DD86BB7500914",
        "desc": "DEMO1 SHOP"
      },
      {
        "id": 2,
        "date_added": "2020-11-03 22:38:58",
        "name": "DEMO2",
        "url": "https://demo2",
        "status": 0,
        "public_key": "1913EA935149B1E5D852A",
        "desc": "DEMO2 SHOP"
      }
    ]
  }
}
```

### Пример запроса
```
{
  "shop_id": "1913EA935149B1E5D852A",
  "nonce": 1613435880
}
```
## <a name="balance"></a>Баланс

    POST https://tegro.money/api/balance/
    
Получение баланса всех кошельков

### Запрос


| Header | type | desc |
|-----------|-----------|-----------|
| Authorization		 | string | Подпись запроса |

| Body | type | desc |
|-----------|-----------|-----------|
shop_id |	string |	Shop ID |
nonce	 |integer	 |Уникальный номер запроса |

### Ответ

```
{
  "type": "success",
  "desc": "",
  "data": {
    "user_id": 1,
    "balance": {
      "RUB": "1396.68",
      "USD": "0.00",
      "EUR": "1.23",
      "UAH": "0.00"
    }
  }
}
```

### Пример запроса
```
{
  "shop_id": "1913EA935149B1E5D852A",
  "nonce": 1613435880,
  "currency": "RUB",
  "amount": 1200,
  "order_id": "test order",
  "payment_system": 5,
  "fields": {
    "email": "user@email.ru",
    "phone": "79111231212"
  },
  "receipt": {
    "items": [
      {
        "name": "test item 1",
        "count": 1,
        "price": 600
      },
      {
        "name": "test item 2",
        "count": 1,
        "price": 600
      }
    ]
  }
}
```

## <a name="check-order"></a>Проверка заказа

    POST https://tegro.money/api/order/

Получение информации о заказе

### Запрос


| Header | type | desc |
|-----------|-----------|-----------|
| Authorization		 | string | Подпись запроса |

| Body | type | desc |
|-----------|-----------|-----------|
shop_id |	string |	Shop ID |
nonce	 |integer	 |Уникальный номер запроса |
order_id	 |integer	 |Номер платежа tegro.money |
payment_id	 |string	 |или номер платежа магазина |

### Ответ

```
{
  "type": "success",
  "desc": "",
  "data": {
    "id": 1232,
    "date_created": "2020-11-14 23:32:37",
    "date_payed": "2020-11-14 23:33:39",
    "status": 1,
    "payment_system_id": 10,
    "currency_id": 1,
    "amount": "64.18000000",
    "fee": "4.00000000",
    "email": "user@site.ru",
    "test_order": 0,
    "payment_id": "Order #17854"
  }

```

### Пример запроса
```
{
  "shop_id": "1913EA935149B1E5D852A",
  "nonce": 1613435880,
  "payment_id": "test order"
}
```


## <a name="list-orders"></a>Список заказов

    POST https://tegro.money/api/orders/

Получение информации о заказах

### Запрос


| Header | type | desc |
|-----------|-----------|-----------|
| Authorization		 | string | Подпись запроса |

| Body | type | desc |
|-----------|-----------|-----------|
shop_id |	string |	Shop ID |
nonce	 |integer	 |Уникальный номер запроса |
page	 |integer	 |Страница|

### Ответ

```
{
  "type": "success",
  "desc": "",
  "data": [
    {
      "id": 123,
      "date_created": "2020-11-14 23:32:37",
      "date_payed": "2020-11-14 23:33:39",
      "status": 1,
      "payment_system_id": 10,
      "currency_id": 1,
      "amount": "64.18000000",
      "fee": "4.00000000",
      "email": "user@somesite",
      "test_order": 0,
      "payment_id": "Order #4175"
    },
    {
      "id": 124,
      "date_created": "2020-11-14 23:30:05",
      "date_payed": null,
      "status": 0,
      "payment_system_id": 10,
      "currency_id": 1,
      "amount": "64.18000000",
      "fee": "4.00000000",
      "email": "user2@somesite",
      "test_order": 0,
      "payment_id": "Order #4174"
    }
  ]
}
```

### Пример запроса
```
{
  "shop_id": "1913EA935149B1E5D852A",
  "nonce": 1613435880,
  "page": 1
}
```

## <a name="with"></a>Вывод средств

    POST https://tegro.money/api/createWithdrawal/


### Запрос


| Header | type | desc |
|-----------|-----------|-----------|
| Authorization		 | string | Подпись запроса |

| Body | type | desc |
|-----------|-----------|-----------|
shop_id |	string |	Shop ID |
nonce |	integer |	Уникальный номер запроса |
currency |	string |	Валюта RUB / USD / EUR etc |
account |	string |	Номер счета для выплаты |
amount |	number |	Сумма |
payment_id |	string |	Идентификатор вывода |
payment_system |	integer |	Платежная система |


## <a name="list-payout"></a>Список выплат

    POST https://tegro.money/api/withdrawals/

### Запрос

| Header | type | desc |
|-----------|-----------|-----------|
| Authorization		 | string | Подпись запроса |

| Body | type | desc |
|-----------|-----------|-----------|
shop_id |	string |	Shop ID |
nonce |	integer |	Уникальный номер запроса |
page |	integer |	Страница |

## <a name="check-payout"></a>Проверка выплаты

    POST https://tegro.money/api/withdrawal/

### Запрос


| Header | type | desc |
|-----------|-----------|-----------|
| Authorization		 | string | Подпись запроса |

| Body | type | desc |
|-----------|-----------|-----------|
shop_id |	string |	Shop ID |
nonce |	integer |	Уникальный номер запроса |
order_id |	integer |	Номер платежа tegro.money |
payment_id |	string |	или номер платежа магазина |


# Справочная информация

## <a name="p-codes"></a>Коды платежных систем

https://tegro.money/docs/other/payment-system-ids/

## <a name="phone-codes"></a>Коды моб. телефонов

https://tegro.money/docs/other/mobile-codes/

## <a name="code-word"></a>Буквенные коды валют

https://tegro.money/docs/other/currency-codes/

# FAQ

## <a name="tarifs"></a>Тарифы и лимиты

https://tegro.money/docs/faq/tariffs-and-limits/

## <a name="mo-project"></a>Модерация проекта

https://tegro.money/docs/faq/moderation/

## <a name="mass"></a>Массовые выплаты

https://tegro.money/docs/faq/mass-payments/

