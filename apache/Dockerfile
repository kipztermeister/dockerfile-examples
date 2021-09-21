# A basic apache server. To use either add or bind mount content under /var/www
FROM ubuntu:12.04@sha256:18305429afa14ea462f810146ba44d4363ae76e4c8dfc38288cf73aa07485005

MAINTAINER Kimbro Staken version: 0.1

RUN apt-get update && apt-get install -y apache2 && apt-get clean && rm -rf /var/lib/apt/lists/*

ENV APACHE_RUN_USER www-data
ENV APACHE_RUN_GROUP www-data
ENV APACHE_LOG_DIR /var/log/apache2

EXPOSE 80

CMD ["/usr/sbin/apache2", "-D", "FOREGROUND"]
