FROM node:latest AS build

WORKDIR /app

COPY . .

RUN npm install

RUN npm run build

# Serve Application using Nginx Server

FROM nginx:1-alpine-slim

COPY --from=build /app/dist/angular-16-crud/ /usr/share/nginx/html


EXPOSE 80
