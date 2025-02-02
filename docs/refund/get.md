---
layout: default
nav_order: 2
title: "Получение возвратов"
parent: "Работа с возвратом"
---

# Получение списка возвратов

Для получения списка возвратов, необходимо вызвать следующий метод API:

- метод: `GET`
- ресурс: `/v3/filter/api/order/refund-order`
- тело ответа - array of [RefundOrderResponse](/docs/refund/create/#refundorderresponse)

Используя этот метод можно получить список возвратов. Возможно применения фильтров и сортировок.

Пример запроса с фильтром по идентификатору заказа

```
GET /v3/filter/api/order/refund-order?id=01771534-196a-1105-839a-82422289d6d9
```

Пример запроса с фильтром по статусу

```
GET /v3/filter/api/order/refund-order?status=completed
```

Пример запроса с фильтром по идентификатору заказа в учётной системе магазина 

```
GET /v3/filter/api/order/refund-order?merchantOrderId=ORD123456
```


