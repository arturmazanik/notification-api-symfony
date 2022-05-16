docker-symfony-postgre-min
--------------------------
Laravel workspace with `PHP 8.1`, `NGINX 1.20+`, `PostgreSQL 13.6+` and `Laravel 9`.

Initialization
====================================================

1. Clone the project:

        https://github.com/arturmazanik/notification-api-laravel.git

1. Go to the project's folder

        cd src

1. add your existing .env or you may the use default .env from laravel

1. install some vendors

        composer install

1. Return to root and build app with command

        docker-compose --env-file ./src/.env up -d --build site

Using
==============

Using app
--------------------

Exposed ports based from ./src/.env ( i will be using .env_example as a sample)

* app_name - `Laravel` (APP_NAME)
* nginx - `:801` (NGINX_PORT)
* pgsql - `:33061` (DB_PORT)
* php - `:9000`
* redis - `:63791` (REDIS_PORT)
* mailhog - `:10251` (MAIL_PORT)