FROM nginx:1.17.3-alpine

LABEL version="0.0.1"
LABEL author="tian"
LABEL email="developadi@gmail.com"

EXPOSE 80
EXPOSE 443

COPY /nginx/sites/default.vhost /etc/nginx/conf.d/default.conf
RUN mkdir -p /var/www