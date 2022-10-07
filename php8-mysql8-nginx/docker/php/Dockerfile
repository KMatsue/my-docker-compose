FROM php:8.1-fpm

WORKDIR /var/www/html

COPY ./php.ini /usr/local/etc/php/

RUN apt-get update \
    && apt-get install -y libfreetype6-dev libjpeg62-turbo-dev libpng-dev libonig-dev \
    && docker-php-ext-install pdo_mysql mysqli

RUN pecl install xdebug && \
    docker-php-ext-enable xdebug