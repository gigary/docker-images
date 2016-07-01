FROM gigary/base:3.4
MAINTAINER Michael Bui <michael@shopback.com>

RUN apk add --update mysql && rm -rf /var/cache/apk/*

RUN rm -rf /var/lib/mysql/* && mysql_install_db

ADD root /

EXPOSE 3306
