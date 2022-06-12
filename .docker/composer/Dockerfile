ARG PHP_VERSION=7.4
FROM php:${PHP_VERSION}-apache
RUN apt-get update && apt-get install -y \
    git \
    curl \
    zip \
    unzip

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

WORKDIR /var/www
