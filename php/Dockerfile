FROM francarmona/docker-ubuntu16-apache2-php7:latest

EXPOSE 80

ARG livezilla_ver
ARG archive_url

ENV livezilla_ver 8.0.0.8
ENV archive_url ${archive_url:-https://www.livezilla.net/downloads/pubfiles/livezilla_server_${livezilla_ver}.zip}

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
    mysql-client \
    php-mysql \
    && rm -rf /var/lib/apt/lists/*
