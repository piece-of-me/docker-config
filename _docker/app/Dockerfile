FROM php:8.2-fpm

RUN apt-get update && apt-get install -y \
      apt-utils \
      libpq-dev \
      libpng-dev \
      libzip-dev \
      zip unzip \
      git && \
#      libjpeg62-turbo-dev \
#      libfreetype6-dev && \
#      pecl install xdebug && \
#      docker-php-ext-install pdo_mysql && \
#      docker-php-ext-install pdo_pgsql && \
      docker-php-ext-install bcmath && \
#      docker-php-ext-install gd && \
      docker-php-ext-install zip && \
#      docker-php-ext-install exif && \
#      docker-php-ext-enable exif && \
#      docker-php-ext-configure gd --with-freetype --with-jpeg && \
#      docker-php-ext-install gd && \
#      docker-php-ext-enable gd && \
#      docker-php-ext-enable xdebug && \
      apt-get clean && \
      rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

# Install composer
ENV COMPOSER_ALLOW_SUPERUSER=1
RUN curl -sS https://getcomposer.org/installer | php -- \
    --filename=composer \
    --install-dir=/usr/local/bin

WORKDIR /var/www
