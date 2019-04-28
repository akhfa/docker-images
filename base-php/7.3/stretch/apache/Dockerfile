FROM php:7.3-apache-stretch
RUN apt update \
    && apt install zlib1g-dev libzip-dev -y \
    && docker-php-ext-install zip \
    && apt clean
RUN curl https://raw.githubusercontent.com/prasathmani/tinyfilemanager/master/tinyfilemanager.php > /var/www/html/filemanager.php
COPY docker-php-entrypoint /usr/local/bin/
