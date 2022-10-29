FROM php:7-apache
COPY . /var/www/html/
RUN docker-php-ext-install pdo pdo_mysql \
&& apachectl restart \
&& mkdir /var/www/html/uploads \
&& chown www-data:www-data /var/www/html/uploads
EXPOSE 80
