FROM ubuntu:latest

RUN apt-get update -y && apt-get install nginx -y

VOLUME [ "/var/www/html" ]

WORKDIR "/var/www/html"

COPY index.html index.html

ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]

EXPOSE 80