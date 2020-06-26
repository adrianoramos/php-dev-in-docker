# PHP Dev in Docker

A quick way to build a PHP development environment using Docker: PHP-FPM, Nginx, MySQL and phpMyAdmin.

## What's included

* [PHP 5.6](http://php.net/)
* [PHP-FPM](https://php-fpm.org/)
* [Nginx](https://www.nginx.com/)
* [MySQL](https://www.mysql.com/)
* [phpMyAdmin](https://www.phpmyadmin.net/)

## Requirements

* [Docker Engine](https://docs.docker.com/engine/installation/)
* [Docker Compose](https://docs.docker.com/compose/install/)
* [Docker Machine](https://docs.docker.com/machine/)

## Clone, Build and Run

```sh
git clone https://github.com/adrianoramos/php-dev-in-docker.git
cd php-dev-in-docker/
docker-compose build
docker-compose up -d
```

Check out `localhost` or `127.0.0.1` in your browser or access the IP address specified in your Docker Machine (Windows and Mac only). You must see the PHP info page located in the `src` directory. 

To access **phpMyAdmin** open the `8080` port in your browser, eg: `localhost:8080`. Log in using **root** as username and password.

## Stop

```sh
docker-compose stop
```

## Kill

```sh
docker-compose kill
```
