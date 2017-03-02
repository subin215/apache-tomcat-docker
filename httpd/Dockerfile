FROM ubuntu:latest

RUN apt-get update \
	&& apt-get install -y apache2

RUN a2enmod proxy \
	&& a2enmod proxy_ajp \
	&& a2enmod proxy_http \
	&& a2enmod rewrite \
	&& a2enmod deflate \
	&& a2enmod headers \
	&& a2enmod proxy_balancer \
	&& a2enmod proxy_connect

RUN rm /etc/apache2/sites-available/000-default.conf

ADD 000-default.conf /etc/apache2/sites-available/000-default.conf

VOLUME ["/var/log/apache2"]

EXPOSE 80 443

CMD ["apachectl", "-k", "start", "-DFOREGROUND"]
