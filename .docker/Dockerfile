FROM php:5.6-apache

# RUN apk add --update bash 

COPY . /code/app
COPY .docker/vhost.conf /etc/apache2/sites-available/000-default.conf

WORKDIR /code/app

RUN chown -R www-data:www-data /code/app
RUN apt-get update
RUN apt-get install -y libmcrypt-dev
RUN docker-php-ext-install mcrypt 