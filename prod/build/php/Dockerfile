FROM php:8.0.30-fpm

WORKDIR /var/www/html/www

RUN apt-get update \
  && apt-get install -y \
        wait-for-it \
        unzip \
        libfreetype6-dev \
        libjpeg62-turbo-dev \
        libpng-dev \
        libzip-dev \
        libcurl3-dev \
		libwebp-dev \
  && docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp \
  && docker-php-ext-install -j$(nproc) gd zip mysqli curl \
  && docker-php-ext-enable gd zip mysqli curl
