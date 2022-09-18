# Dockerfile
FROM php:8.1-cli

RUN apt-get update -y && apt-get install -y libmcrypt-dev

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
RUN docker-php-ext-install pdo mbstring

WORKDIR /echo-service-symfony-docker
COPY . /echo-service-symfony-docker

RUN composer install

EXPOSE 8000
CMD php bin/console server:run 0.0.0.0:8000
