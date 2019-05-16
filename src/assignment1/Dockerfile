FROM alpine:3.7

RUN apk add nginx \
&& mkdir -p /run/nginx \
&& mkdir /var/www/default

COPY ./nginx/default.conf /etc/nginx/conf.d/default.conf
COPY ./src/index.html /var/www/default/index.html

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]