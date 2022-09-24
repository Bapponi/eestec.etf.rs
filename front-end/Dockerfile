FROM node:lts-alpine3.14

WORKDIR /app

COPY . .

RUN npm install

EXPOSE 8080

ENTRYPOINT [ "npm", "run", "serve" ]