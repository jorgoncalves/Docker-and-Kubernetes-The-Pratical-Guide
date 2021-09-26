FROM node

WORKDIR /app

COPY package.json /app
# . = /app no caso

RUN npm install

COPY . /app
#. ou /app. . referece ao workdir

EXPOSE 3000

CMD ["node", "server.js"]

