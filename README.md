![example workflow](https://github.com/Mind-Insight/kittygram_final/actions/workflows/main.yml/badge.svg)

# Kittygram

Данный проект дает возможность пользователям публиковать информацию о своих котах. Есть возможность
регистрации на сайте. Зарегистрированные пользователи могут полностью управлять своими записями.

## Стек технологий

- Python
- Django
- Gunicorn
- Docker
- DRF
- Nginx

## Развертывание проекта

1. Клонировать репозиторий:

```
git clone https://github.com/your/repository.git
```

2. Создать и активировать виртуальное окружение
```
python3 -m venv venv
source venv/bin/activate
```

3. Установить зависимости:

```
pip install -r backend/requirements.txt
```

4. В корне проекта создать .env
```
nano .env
```
и заполнить его содержимым .env.example

5. Запустите проект локально
```
sudo docker compose up
```

6. Выполните миграции следующей командой
```
sudo docker exec kittygram_final_backend_1 python manage.py migrate
```

7. Перейдите по ссылке http://0.0.0.0:9000

## Автор

Автор проекта: [Timofey Averchenkov](https://github.com/Mind-Insight)