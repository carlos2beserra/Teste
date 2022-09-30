FROM node:10-alpine

WORKDIR /home/node/app

RUN mkdir -p /home/node/app/node_modules && chown -R node:node /home/node/app

COPY --from=build /home/node/app/.env ./

EXPOSE 8080

RUN npm install 
