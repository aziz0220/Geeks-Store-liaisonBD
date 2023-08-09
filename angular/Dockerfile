FROM --platform=$BUILDPLATFORM node:16.20.1-alpine3.18 as build-step

WORKDIR /app

COPY package.js ./

RUN npm install -g @angular/cli

RUN npm ci

COPY . .

EXPOSE 4200

CMD npm run start
