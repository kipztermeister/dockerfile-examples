# A basic apache server with PHP. To use either add or bind mount content under /var/www

FROM kstaken/apache2:latest@sha256:50f87db6688529491d734fdb515600d96d20a13df2b1e9215812aff8a47c040e

MAINTAINER Kimbro Staken version: 0.1

RUN apt-get update && apt-get install -y php5 libapache2-mod-php5 php5-mysql php5-cli && apt-get clean && rm -rf /var/lib/apt/lists/*

CMD ["/usr/sbin/apache2", "-D", "FOREGROUND"]
