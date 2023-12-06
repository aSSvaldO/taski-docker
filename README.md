# Kittygram final

## Описание
Проект Kittygram представляет собой веб-платформу для любителей кошек, где владельцы могут публиковать информацию о своих питомцах, включая имя, окрас, дату рождения, фотографии, а также делиться достижениями своих питомцев. Создание данного ресурса позволяет владельцам кошек составить реестр своих любимцев.

## Запуск
Для запуска приложения необходим сервер, рассмотрим на примере сервера под управлением ОС Linux.

1. Подготовим виртуальное окружение в директории проекта создадим файл .env:
```bash
nano .env
```

2. Добавляем следующие переменные:
```nano
POSTGRES_DB=kittygram
POSTGRES_USER=kittygram_user
POSTGRES_PASSWORD=kittygram_password
DB_HOST=db
DB_PORT=5432
DEBUG=False
```

3. Устанавливаем к Docker утилиту Docker Compose:
```bash
sudo apt update
sudo apt-get install docker-compose-plugin 
```

4. В директорию проекта копируем файл `docker-compose.production.yml` и запускаем Docker Compose:
```bash
sudo docker-compose up
```
## Об авторе
Илья Бородин