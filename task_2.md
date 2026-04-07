# Пример REST API запроса

```http
GET /api/v1/partner-stores?cityId=1&lat=55.7558&lon=37.6176 HTTP/1.1
Host: api.petrushka-green.ru
Authorization: Bearer <token>
Accept: application/json
X-Platform: ios
X-App-Version: 5.12.0
```

# Пример ответа API

```json
{
  "status": "success",
  "timestamp": "2026-04-07T09:41:00Z",
  "data": {
    "title": "Выберите магазин",
    "stores": [
      {
        "id": "metro",
        "name": "METRO",
        "logoUrl": "https://cdn.petrushka-green.ru/partners/metro/logo.png",
        "delivery": {
          "type": "nearest",
          "label": "Ближайшая доставка",
          "timeText": "сегодня 21:00-23:00"
        },
        "backgroundColor": "#FFFFFF",
        "externalUrl": "https://online.metro-cc.ru/",
        "isAvailable": true,
        "sortOrder": 1
      },
      {
        "id": "auchan",
        "name": "Ашан",
        "logoUrl": "https://cdn.petrushka-green.ru/partners/auchan/logo.png",
        "delivery": {
          "type": "nearest",
          "label": "Ближайшая доставка",
          "timeText": "сегодня 18:00-20:00"
        },
        "backgroundColor": "#FFFFFF",
        "externalUrl": "https://www.auchan.ru/",
        "isAvailable": true,
        "sortOrder": 2
      },
      {
        "id": "vkusvill",
        "name": "ВкусВилл",
        "logoUrl": "https://cdn.petrushka-green.ru/partners/vkusvill/logo.png",
        "delivery": {
          "type": "fast",
          "label": "Быстрая доставка",
          "timeText": "от 20 до 60 минут"
        },
        "backgroundColor": "#FFFFFF",
        "externalUrl": "https://vkusvill.ru/",
        "isAvailable": true,
        "sortOrder": 3
      },
      {
        "id": "victoria",
        "name": "ВИКТОРИЯ",
        "logoUrl": "https://cdn.petrushka-green.ru/partners/victoria/logo.png",
        "delivery": {
          "type": "nearest",
          "label": "Ближайшая доставка",
          "timeText": "сегодня 17:00-19:00"
        },
        "backgroundColor": "#C8E63C",
        "externalUrl": "https://victoria-group.ru/",
        "isAvailable": true,
        "sortOrder": 4
      }
    ]
  }
}
```
