FROM node:alpine

#set working directory inside pod
WORKDIR /usr/app

#copy package.json of simpleweb
COPY ./simpleweb/package.json ./

#install dependencies
RUN npm install

#copy rest of the contents of simpleweb
COPY ./simpleweb/ ./

#Command
CMD ["npm", "start"]

