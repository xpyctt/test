FROM php:7.4-fpm

RUN \
    apt-get update && \
    apt-get install -y --no-install-recommends \
        vim \
        ssh \
        default-mysql-client \
    && pecl install xdebug \
    && docker-php-ext-enable xdebug \
    && docker-php-ext-install pdo_mysql