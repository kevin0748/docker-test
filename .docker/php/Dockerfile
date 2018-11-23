FROM php:5.6.38-fpm-alpine

RUN apk update \
    apk upgrade

RUN apk add libmcrypt-dev
RUN docker-php-ext-install mcrypt 
