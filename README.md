# REST API на Node.js 

**Используемые технологии**

* Node.js
* express.js
* sqllite

**Доступные маршруты**

`GET /api/articles` — получить все статьи
`GET /api/article/:id` — получить конкретную статью по id
`POST /api/article` — создать статью
`PUT /api/article/:id` — редактировать статью
`DELETE /api/article/:id` — удалить статью по id


## Общее впечатление ##
* Задание выполнено довольно грамотно. Все 5 запросов работают корректно. Ошибки обрабатываются должным образом и формирются ответы об ошибке
(например error: "title обязательно"). Коды ошибок соответствуют спецификации https://developer.mozilla.org/ru/docs/Web/HTTP/Status
В запросах добавления в БД записей правильно используется параметризованный запрос - нет возможности провести sql injection.

## Замечания ##

** package.json **
* Необходимо обновить до последних версий все пакеты из [dependencies](https://github.com/OriginalSin/code-reView-node/blob/main/package.json#L12)
Например:
  "dependencies": {
    "express": "^4.17.1",
    "lodash": "^4.17.21",
    "md5": "^2.3.0",
    "sqlite3": "^5.0.2"
  }
