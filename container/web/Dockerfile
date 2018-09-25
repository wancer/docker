FROM php:fpm-alpine

RUN apk --no-cache add nginx

RUN rm /etc/nginx/conf.d/default.conf
COPY ./conf.d /etc/nginx/conf.d/
RUN mkdir -p /run/nginx

EXPOSE 80

CMD ["sh", "-c", "nginx && php-fpm"]
