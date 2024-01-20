Первые шаги по запуску проекта я делал в проекте zero

Далее:

Настроить конфигурацию: в этом проекте конфигурация находиться по адресу: ввести адрес

Инициализация проекта:

Запуск контейнера php (docker):
docker exec -it oop-php-1 bash

В контейнере вводим команду:
php init (это инициализация yii проекта в самом проекте есть файл init (в котором прописал скрипт php), также есть файл init.bat для windows)

Проверить настройки БД (имя БД, логин, пароль):
/path/to/yii-application/common/config/main-local.php

Создать базу данных (я создавал в MySQL Workbench)

Проверить подключение к базе данных

# zero

Это чистый проект на технологиях docker/nginx/php/mysql. Необходим для разработки нового проекта с нуля на docker.

Сделать полное описание каждого файла в структуре этого проекта на технологиях: docker/nginx/php/mysql

Стандартные репозитории и файлы для нового проекта на docker:

<img width="180" alt="index php" src="https://github.com/al-zv/zero/assets/63869857/77fd833a-1d9b-4e59-96e5-4f60e80f1e69">

zero - наименование репозитория проекта

zero/docker-compose.yml - главный файл docker


zero/nginx - репозиторий для настроек веб-сервера nginx

zero/nginx/core - репозиторий для настроек веб-сервера nginx

zero/nginx/core/nginx.conf - файл с настройками веб-сервера nginx


zero/nginx/www/app - репозиторий с кодом проекта

zero/nginx/www/app/index.php - индексный файл php для проверки работы docker


zero/php - репозиторий с настройками PHP для docker

zero/php/Dockerfile - файл с настройками PHP для docker

### <a name="21">1. Инструкция по запуску проекта</a> 

Скачать с GitHub

    git clone https://github.com/al-zv/zero.git
