FROM php:8.2-apache
WORKDIR /var/www/html
RUN apt-get update && apt-get install -y \
                libzip-dev \
                zlib1g-dev \
                libfreetype-dev \
                libjpeg62-turbo-dev \
                libpng-dev \
        && docker-php-ext-configure gd --with-freetype --with-jpeg \
        && docker-php-ext-install -j$(nproc) zip gd mysqli