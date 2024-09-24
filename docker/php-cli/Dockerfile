FROM php:8.2-cli

RUN apt-get update && apt-get install -y \
    libpq-dev \
    wget \
    zlib1g-dev \
    libmcrypt-dev \
    libzip-dev

RUN docker-php-ext-install pdo pdo_mysql zip curl fileinfo mbstring exif openssl pdo_sqlite

RUN wget https://getcomposer.org/installer -O - -q | php -- --install-dir=/bin --filename=composer --quiet

RUN composer install

WORKDIR /symfony