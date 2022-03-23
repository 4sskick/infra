FROM php:7.4.2-fpm

LABEL version="0.0.1"
LABEL author="tian"
LABEL email="developadi@gmail.com"

RUN apt-get -y update && \
    apt-get install -y libpq-dev \
    libonig-dev \
    libicu-dev

RUN docker-php-ext-install pdo_mysql && \
    docker-php-ext-install mbstring && \
    docker-php-ext-install mysqli && \
    docker-php-ext-install bcmath && \
    docker-php-ext-configure intl && \
    docker-php-ext-install intl && \
    docker-php-ext-install curl && \
    docker-php-ext-install fileinfo && \
    docker-php-ext-install pdo && \
    docker-php-ext-install dom && \
    docker-php-ext-install json && \
    docker-php-ext-install tokenizer && \
    docker-php-ext-install xml && \
    docker-php-ext-install ctype && \
    docker-php-ext-install bcmath

# RUN pecl install redis && \
#     rm -rf /tmp/pear && \
#     docker-php-ext-enable redis

RUN docker-php-ext-install sockets
COPY /php/php.ini /etc/php/7.4/fpm/conf.d/40-custom.ini

EXPOSE 9000