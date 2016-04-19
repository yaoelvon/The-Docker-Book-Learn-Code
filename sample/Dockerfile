FROM ubuntu:14.04
MAINTAINER Feng Yao "me@fengyao.me"
ENV PEFRESHED_AT 2016-04-19
RUN apt-get update
RUN apt-get install -y -q nginx
RUN mkdir -p /var/www/html
ADD nginx/global.conf /etc/nginx/conf.d/
ADD nginx/nginx.conf /etc/nginx/nginx.conf
EXPOSE 80

# ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]