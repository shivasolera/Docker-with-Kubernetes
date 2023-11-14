FROM node:14

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

# giving the port number to the container.
ENV PORT=80


# VOLUME [ "/app/feedback" ] we can remove this because we add this as a unnamed volume 

#EXPOSE 80
#using below we can expose multiple ports
EXPOSE $PORT

#CMD [ "node", "server.js" ]

# this command because we added nodemon to the package.json. which will start the node server.
# it restarts the server when we make changes to the code.
CMD [ "npm", "start" ]