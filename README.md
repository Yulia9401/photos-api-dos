# JSON Placeholder photos API
## 📚 Описание

Документация к REST API для работы с книгами (на базе мокового сервиса).  
Цель: зафиксировать контракт API (эндпоинты, методы, статусы, структура данных) для интеграции и проектирования БД.

## 🔮 Возможности

- **GET /photos** — получить список фото. Статус: 200 OK. Возвращает массив объектов.
- **GET /photos/{id}** — получить фото по ID. Статус: 200 OK или 404 Not Found.
- **POST /books** — добавить фото. Статус: 201 Created. В теле — данные фото.
- **PUT /photos/{id}** — полностью обновить данные о фото. Статус: 200 OK. Требуется полный объект.
- **PATCH /photos/{id}** — частично обновить данные о фото. Статус: 200 OK. Только изменённые поля.
- **DELETE /photos/{id}** — удалить фото. Статус: 200 OK (в моке — эмуляция).

## 💎 Технологии
- REST API
- [OpenAPI 3.0 (спецификация контракта)](https://editor.swagger.io/?url=https://raw.githubusercontent.com/Yulia9401/photos-api-dos/main/openapi.yaml)
- Swagger UI (визуализация через [editor.swagger.io](https://editor.swagger.io/?url=https://raw.githubusercontent.com/Yulia9401/photos-api-dos/main/openapi.yaml))
- Postman — тестирование и коллекции запросов


## 🌐 Быстрые ссылки

- Swagger UI: [editor.swagger.io](https://editor.swagger.io/) (вставить `photos_api.yaml` в редактор)
- Postman коллекция: файл `photos-api.postman_collection.json` в репозитории
- Mock Server: будет опубликован позже

## 📖 API Endpoints

| Метод | Эндпоинт | Описание | Статус |
|-------|----------|----------|--------|
| GET | `/photos` | Список книг | 200 |
| GET | `/photos/{id}` | Книга по ID | 200/404 |
| POST | `/photos` | Создать книгу | 201 |
| PUT | `/photos/{id}` | Полное обновление | 200 |
| PATCH | `/photos/{id}` | Частичное обновление | 200 |
| DELETE | `/photos/{id}` | Удалить книгу | 200 |

## ⚡ Пример запроса

Пример вызова к Postman Mock Server:

curl -v https://jsonplaceholder.typicode.com/photos
