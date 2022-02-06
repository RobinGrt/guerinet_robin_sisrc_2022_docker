FROM node:12.18-alpine

RUN mkdir /usr/app

WORKDIR /usr/app

RUN npm install -g nodemon

COPY package.json /usr/app/package.json

COPY yarn.lock /usr/app/yarn.lock

RUN yarn install

COPY . .

EXPOSE 8080

EXPOSE 27017

CMD ["nodemon","server"]
