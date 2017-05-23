FROM ubuntu
MAINTAINER Stefan Liu

RUN apt-get install -y software-properties-common python
RUN add-apt-repository ppa:chris-lea/node.js
RUN echo "deb http://us.archive.ubuntu.com/ubuntu/ precise universe" >> /etc/apt/sources.list
RUN apt-get update && apt-get install -y nodejs
#RUN apt-get install -y nodejs=0.6.12~dfsg1-1ubuntu1
RUN mkdir /var/www

ADD WebTerminal /var/www/

RUN cd /var/www/WebTerminal/ && /usr/bin/npm install

CMD ["/usr/bin/node", "/var/www/WebTerminal/bin/tty.js", "/var/www/WebTerminal/config.json"]
