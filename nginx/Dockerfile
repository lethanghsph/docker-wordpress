FROM nginx:latest

MAINTAINER Le Tien Thang <lethanghsph@gmail.com>

ENV TERM xterm
COPY nginx.conf /etc/nginx/nginx.conf
COPY default.conf /etc/nginx/conf.d/default.conf
COPY upstream.conf /etc/nginx/conf.d/upstream.conf
RUN usermod -u 1000 www-data
RUN mkdir -p /var/www/wordpress/ \
    && touch /var/www/wordpress/index.php

CMD ["nginx"]

EXPOSE 80 443
