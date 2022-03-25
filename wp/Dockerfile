FROM wordpress:latest

COPY apm-agent-php_1.4.2_all.deb /tmp/apm-agent-php_1.4.2_all.deb

#for alpine
#RUN apk add --allow-untrusted /tmp/apm-agent-php_1.4.2_all.apk

RUN dpkg -i /tmp/apm-agent-php_1.4.2_all.deb

COPY 99-elastic-apm-custom.ini /usr/local/etc/php/conf.d/zzzzzz-elastic-apm-custom.ini
