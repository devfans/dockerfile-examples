FROM node:alpine

MAINTAINER Stefan Liu

RUN mkdir /var/www

COPY WebTerminal /var/www/

WORKDIR /var/www/WebTerminal

RUN npm install

EXPOSE 9999/tcp

CMD ["node", "bin/tty.js", "config.json"]
