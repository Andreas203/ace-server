FROM node:latest
WORKDIR /
COPY package*.json ./
COPY tsconfig*.json ./

COPY ./src/main ./app

RUN npm install -g ts-node
RUN yarn install

EXPOSE 3000
  
CMD ["ts-node", "/app/server.ts"]
