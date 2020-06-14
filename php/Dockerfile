ARG PHP_VERSION=""
FROM php:${PHP_VERSION:+${PHP_VERSION}-}fpm-alpine

RUN apk update; \
    apk upgrade; 

RUN docker-php-ext-install mysqli

RUN curl --silent --show-error https://getcomposer.org/installer | php && \
    mv composer.phar /usr/local/bin/composer

# install phpunit
RUN wget https://phar.phpunit.de/phpunit-9.0.phar && \
    chmod +x phpunit-9.0.phar && \
    mv phpunit-9.0.phar /usr/local/bin/phpunit