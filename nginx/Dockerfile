FROM gigary/base:3.4
MAINTAINER Michael Bui <mf.michaelbui@gmail.com>

RUN apk add --update nginx
RUN rm -rf /var/cache/apk/*

ADD root /

EXPOSE 80

VOLUME "/var/www"

RUN mkdir -p /var/www/public

RUN chown -R nginx:www-data /var/www
