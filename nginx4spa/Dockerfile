# NAME:  shebgregor/nginx4spa
FROM nginx

LABEL maintainer "Michael Popsuev <sheb.gregor@gmail.com>"

RUN rm /etc/nginx/conf.d/*.conf
COPY ./spa.conf /etc/nginx/conf.d/
