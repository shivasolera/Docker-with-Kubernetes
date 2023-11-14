FROM node

WORKDIR /app2

COPY package.json /app2

RUN npm install

COPY . /app2

EXPOSE 3000

CMD [ "node", "server.js" ]
