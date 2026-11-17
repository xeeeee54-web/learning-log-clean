
# Learning Log

Учебный проект на Django. Сайт позволяет создавать темы и добавлять к ним записи.

## Используемые технологии

- Python
- Django
- SQLite
- Gunicorn
- WhiteNoise
- Docker Compose

## Запуск на локальном компьютере

1. Установить зависимости:

   ```powershell
   pip install -r requirements.txt
   ```

2. Выполнить миграции:

   ```powershell
   python manage.py migrate
   ```

3. Запустить сервер:

   ```powershell
   python manage.py runserver
   ```

4. Открыть в браузере:

   http://127.0.0.1:8000/

## Запуск на сервере

Проект запускается с помощью Docker Compose.

```bash
docker compose up -d --build
```

При запуске контейнера автоматически выполняются миграции базы данных и сбор статических файлов.

