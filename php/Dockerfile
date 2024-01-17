FROM php:8.1.1-apache
RUN apt-get update \
&& apt-get install -y libonig-dev libzip-dev unzip\
&& docker-php-ext-install pdo_mysql mbstring zip bcmath\
&& pecl install xdebug\
&& docker-php-ext-enable xdebug

COPY --from=composer /usr/bin/composer /usr/bin/composer
WORKDIR /usr/src/myapp

RUN echo "ServerName localhost" | tee /etc/apache2/conf-available/fqdn.conf
RUN a2enconf fqdn
