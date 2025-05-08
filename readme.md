# Домашнє завдання — Тема 2. Розгортання FastAPI-застосунку в Docker

## Що реалізовано:

- Клоновано репозиторій FastAPI-застосунку
- Створено `Dockerfile` з використанням Python 3.10
- Написано `docker-compose.yaml` з конфігурацією для FastAPI та PostgreSQL
- Внесено зміни до `conf/db.py` для правильного підключення до БД через ім’я сервісу `db`
- Використано `docker-compose up --build` для запуску
- Перевірено роботу застосунку: головна сторінка працює, перевірка БД проходить успішно

## Сервіси:

- **web** — FastAPI застосунок, порт 8000
- **db** — PostgreSQL 13, порт 5432

## Структура проєкту:

```bash
FullStack-Web-Development-hw2/
├── conf/
│   └── db.py               # Підключення до бази
├── static/                 # Статичні файли
├── templates/              # HTML шаблони
├── main.py                 # FastAPI застосунок
├── requirements.txt        # Залежності
├── Dockerfile              # Docker інструкції
├── docker-compose.yaml     # Конфігурація середовища
```
bash
Копировать
Редактировать

## Як запустити:

```bash
git clone https://github.com/GoIT-Python-Web/FullStack-Web-Development-hw2
cd FullStack-Web-Development-hw2
docker-compose up --build
```
