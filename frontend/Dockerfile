FROM node:18-alpine as builder
WORKDIR /app
COPY package*.json ./
RUN npm ci --no-audit --no-fund
COPY . ./
ENTRYPOINT [ "npm", "run", "start" ]