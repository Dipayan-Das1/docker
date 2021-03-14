FROM node:alpine

WORKDIR /usr/app

COPY ./visits-app/package.json ./

RUN npm install

COPY ./visits-app/ ./

CMD ["npm","start"]