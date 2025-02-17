backend/
├── app/
│   ├── main.py          # Основной файл API
│   ├── database.py      # Настройка БД
│   ├── models.py        # Модели SQLAlchemy
│   └── schemas.py       # Схемы Pydantic
└── tasks.db             # Файл базы данных

CRUD для задач:

GET /tasks – список всех задач.
GET /tasks/{id} – задача по ID.
POST /tasks – создать задачу.
PUT /tasks/{id} – обновить задачу.
DELETE /tasks/{id} – удалить задачу.
Валидация данных через Pydantic.
Автоматическая документация (Swagger).
База данных: SQLite с использованием SQLAlchemy.

Перед началом работы 
Установить зависимости
pip install -r requirements.txt

 Запустить сервер
uvicorn app.main:app --reload
Бэкенд будет доступен на http://localhost:8000