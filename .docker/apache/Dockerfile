FROM httpd:2.4-alpine

RUN apk update; \
    apk upgrade;

COPY vhost.conf /usr/local/apache2/conf/extra/vhosts.conf
RUN echo "Include /usr/local/apache2/conf/extra/vhosts.conf" \
    >> /usr/local/apache2/conf/httpd.conf