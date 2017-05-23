FROM node:4-onbuild

MAINTAINER Stefan Liu

RUN mkdir /var/www

COPY WebTerminal /var/www/

RUN cd /var/www/WebTerminal/ && /usr/bin/npm install

EXPOSE 9999

CMD ["/usr/bin/node", "/var/www/WebTerminal/bin/tty.js", "/var/www/WebTerminal/config.json"]
