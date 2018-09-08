FROM php:7.2-fpm
RUN apt-get update && apt-get install -y \
git \
zip \
unzip
RUN docker-php-ext-install pdo pdo_mysql
RUN pecl install xdebug \
&& docker-php-ext-enable xdebug

COPY config/php.ini /usr/local/etc/php/
