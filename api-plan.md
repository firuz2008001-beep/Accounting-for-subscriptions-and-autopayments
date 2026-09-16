# План API

## Базовый URL: `/api/v1`

### Подписки
- `GET /subscriptions` — получить список всех подписок.
- `POST /subscriptions` — добавить новую подписку.
- `GET /subscriptions/{id}` — получить детали конкретной подписки.
- `PUT /subscriptions/{id}` — обновить подписку.
- `DELETE /subscriptions/{id}` — удалить (отменить) подписку.

### Платежи
- `GET /payments/upcoming` — получить список предстоящих списаний.
- `POST /payments/{id}/pay` — провести ручной платеж (если автоплатеж не сработал).

### Пример запроса на создание подписки (JSON)
```json
{
  "title": "Яндекс.Плюс",
  "amount": 399,
  "currency": "RUB",
  "period": "monthly",
  "next_payment_date": "2023-12-01"
}
<<<<<<< HEAD
## Эндпоинты для работы со списком подписок
- `GET /api/v1/subscriptions` — получить список всех активных подписок пользователя.
- `GET /api/v1/subscriptions/{id}` — получить детали конкретной подписки.
- `POST /api/v1/subscriptions` — добавить новую подписку в трекер.
=======
>>>>>>> 96b4dd69e4b8e79e7e046a2316415ba0389c552c
