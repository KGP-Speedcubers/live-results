FROM node:18-alpine

# setup pnpm
WORKDIR /app
RUN npm install -g pnpm@latest-10

# install dependencies
COPY package.json /app/
COPY pnpm-lock.yaml /app/
RUN pnpm install

# copy sources
COPY . /app/
EXPOSE 5173

# run
CMD ["pnpm", "run", "dev"]
