FROM nextcloud:fpm-alpine

RUN apk add --no-cache --virtual .build-deps samba-dev $PHPIZE_DEPS && \
    apk add samba-client && \
    pecl install smbclient && \
    docker-php-ext-enable smbclient && \
    apk del .build-deps

COPY redis.config.php /usr/src/nextcloud/config/redis.config.php
