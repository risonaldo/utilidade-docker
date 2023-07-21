FROM php:7.4-apache

WORKDIR /var/www/html

RUN apt-get update && apt-get install -y

RUN a2enmod rewrite
RUN apache2ctl stop && apache2ctl start

RUN docker-php-ext-install pdo 
RUN docker-php-ext-install pdo_mysql
RUN docker-php-ext-install mysqli 
RUN docker-php-ext-install mysql
