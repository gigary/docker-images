FROM alpine:3.4
MAINTAINER Michael Bui <mf.michaelbui@gmail.com>

RUN apk add --update php5-cli php5-mysql php5-pdo_mysql php5-mcrypt php5-curl php5-json php5-ctype php5-zlib php5-dom php5-xml php5-openssl

RUN apk add --update --repository http://dl-3.alpinelinux.org/alpine/edge/testing/ --allow-untrusted php5-phar

RUN rm -rf /var/cache/apk/*

ADD root /
RUN ln -sf /phpunit.phar /usr/bin/phpunit
RUN chmod +x /phpunit.phar
RUN chmod +x /usr/bin/phpunit
