FROM craigbeck/node-nginx

RUN mkdir /app
WORKDIR /app

ONBUILD COPY package.json /app/
ONBUILD RUN npm install
ONBUILD COPY . /app/
ONBUILD RUN webpack -p

ENV NODE_ENV production
