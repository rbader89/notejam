FROM node

WORKDIR /usr/src/app

COPY . .

WORKDIR /usr/src/app/notejam

RUN npm install

RUN node ./db.js

CMD ["./bin/www"]