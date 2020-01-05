FROM node:12.2.0-alpine

WORKDIR /app

# install and cache app dependencies
COPY package.json /app/package.json

RUN npm install --silent

RUN apk update \
    && apk upgrade \
    && apk add bash

CMD ["node", "index.js"]