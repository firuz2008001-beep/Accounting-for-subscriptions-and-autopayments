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
