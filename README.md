
## Базовый пример FastAPI + Aiosqlite c CRUD операциями

### Описание
- В примере представлены простые операции для работы с базой данных sqlite в асинхронном режиме.
- В менеджере сессий используется @asynccontextmanager - это гарантирует, что соединение с БД будет закрыто после завершения запроса.
- В примере не используется ORM и пул соединений.

### Структура

```
./
├── app
│   ├── database.py
│   ├── main.py
│   ├── models.py
│   ├── routes
│   │   ├── api.py
│   │   └── frontend.py
│   ├── static
│   │   ├── css
│   │   │   └── default.css
│   │   ├── images
│   │   │   └── favicon.ico
│   │   └── js
│   │       └── default.js
│   └── templates
│       ├── 404.html
│       └── index.html
├── README.md
└── requirements.txt
```