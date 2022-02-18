FROM php:7.4-apache

LABEL version="0.0.1"
LABEL author="tian"
LABEL email="developadi@gmail.com"

RUN docker-php-ext-install mysqli

#install composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

#copy --from=<image_docker> /src /dst
# COPY --from=composer:latest /usr/bin/composer /usr/bin/composer