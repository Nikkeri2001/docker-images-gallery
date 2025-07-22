FROM node:16.8.0-alpine

WORKDIR /app

EXPOSE 3000

COPY package*.json ./

RUN npm install --silent


COPY . ./

CMD [ "npm", "start" ]
