FROM php:8.3.3-fpm

RUN apt-get update && apt-get install -y git zip unzip \
    && docker-php-ext-install pdo_mysql

#Composer install
RUN php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');" \
    && php composer-setup.php \
    && php -r "unlink('composer-setup.php');" \
    && mv composer.phar /usr/local/bin/composer


WORKDIR /var/www/
