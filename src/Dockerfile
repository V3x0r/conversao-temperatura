FROM node

RUN apt update -y 

RUN useradd Container

WORKDIR /app

COPY package*.json  .

RUN npm install

COPY . .

ENTRYPOINT [ "node", "server.js" ]

EXPOSE 8080

USER Container






