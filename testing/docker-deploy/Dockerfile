FROM node:13.12-alpine3.10

WORKDIR /usr/src/app

COPY package*.json ./
RUN npm ci --only=production
COPY . .

EXPOSE 3000

ENTRYPOINT ["node","index.js"]
