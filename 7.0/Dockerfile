FROM php:7.0.4-fpm

MAINTAINER Personare <devops@personare.com.br>

RUN apt-get update && apt-get install -y \
    git \
    curl \
    unzip \
    && docker-php-ext-install mysqli pdo pdo_mysql \
    && rm -rf /var/lib/apt/lists/*

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

WORKDIR /var/www/html
