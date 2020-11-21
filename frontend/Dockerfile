#build phase
#use node apline
FROM node:alpine as builder
WORKDIR /app
COPY package.json .
RUN npm install
COPY . .
RUN npm run build

#run phase
FROM nginx
#copy contents of build phase from /app/build directory to nginx
COPY --from=builder /app/build /usr/share/nginx/html
#docker run -p 8080:80 dipayandas1/nginx-node:latest





