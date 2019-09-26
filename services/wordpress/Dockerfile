FROM wordpress:5-php7.3-fpm-alpine

RUN set -ex \
  && apk add --no-cache --virtual .build-deps $PHPIZE_DEPS \
  && pecl install xdebug \
  && apk del .build-deps