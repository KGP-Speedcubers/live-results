FROM node:18

# install dependencies
WORKDIR /app
COPY package*.json /app/
RUN npm install

# copy .env and sources
COPY . /app/

# run
EXPOSE 5000
CMD ["node", "server.js"]
