FROM node:0.12

RUN npm install -g cnpm gulp bower && npm cache clear

WORKDIR /opt
EXPOSE 8001
VOLUME ["/opt"]

CMD node /opt/htdocs/broadcast/app.js 8001
