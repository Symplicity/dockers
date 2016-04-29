FROM iron/base

RUN echo '@testing http://nl.alpinelinux.org/alpine/edge/testing' >> /etc/apk/repositories

RUN apk update && apk upgrade \
  && apk add php7@testing php7-openssl@testing php7-phar@testing php7-json@testing php7-curl@testing php7-mbstring@testing \
  php7-intl@testing php7-ldap@testing php7-mcrypt@testing php7-mysqlnd@testing php7-posix@testing php7-pdo_sqlite@testing \
  php7-redis@testing php7-sqlite3@testing php7-sockets@testing php7-tidy@testing php7-zip@testing \
  && rm -rf /var/cache/apk/*

RUN ln -s /usr/bin/php7 /usr/bin/php
