FROM node

RUN apt update -y 
RUN useradd Container
WORKDIR /app

COPY . /app

RUN npm install

ENTRYPOINT [ "node", "server.js" ]

EXPOSE 8080
USER Container






