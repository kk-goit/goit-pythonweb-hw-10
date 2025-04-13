# goit-pythonweb-hw-10
Тема 10. Домашня робота

## Dockerized
Для запуску потрібно виконати команду
```sh
docker-compose --env-file .env-docker up --build
```

## Налаштування
Для зберігання налаштувань необхідно редагувати файл .env-docker
```sh
BIND_HOST=0.0.0.0

DB_TYPE=postgresql+asyncpg
DB_USER=postgres
DB_PASS=qwerty
DB_HOST=dbm
DB_PORT=5432
DB_NAME=hw10

DB_URL=${DB_TYPE}://${DB_USER}:${DB_PASS}@${DB_HOST}:${DB_PORT}/${DB_NAME}

REDIS_URL=redis://redis

SECRET_KEY=Qk4OQQX7Mcdlokb57qk

MAIL_USERNAME=kkondor.goit@meta.ua
MAIL_FROM=${MAIL_USERNAME}
MAIL_PASSWORD=*********

CLOUDINARY_NAME=dueyvjvwx
CLOUDINARY_API_KEY=768168183694751
CLOUDINARY_API_SECRET=Me8VVznKwYBj1v5uxbyZo28J1iY
```
Файл .env викорстовуэться виключно для розробки