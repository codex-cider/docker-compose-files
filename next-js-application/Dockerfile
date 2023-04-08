FROM node:16-alpine
# change node version as your requirement

RUN mkdir -p /usr/app/
WORKDIR /usr/app

COPY package.json .
RUN npm i --force

COPY . .
RUN npm run build

EXPOSE 3000
CMD ["npm","start"]