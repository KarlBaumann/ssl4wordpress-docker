FROM wordpress:latest

RUN apt update \
    && apt upgrade -y \
    && apt install mc -y \
    && pecl install "xdebug" \
    && docker-php-ext-enable xdebug \
    && a2ensite default-ssl \
    && a2enmod ssl \
    && apt install ssl-cert -y \
    && service apache2 restart


