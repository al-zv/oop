# Базовый образ
FROM php:7.4-fpm

# эта строчка нужна чтобы устанавливались php расширения
COPY --from=mlocati/php-extension-installer /usr/bin/install-php-extensions /usr/local/bin/

# Установка расширений
RUN install-php-extensions zip 
RUN install-php-extensions pdo_mysql 
RUN install-php-extensions gd 
RUN install-php-extensions exif

# Установка composer
RUN curl -sS https://getcomposer.org/installer | php && mv composer.phar /usr/local/bin/composer

WORKDIR /var/www/app