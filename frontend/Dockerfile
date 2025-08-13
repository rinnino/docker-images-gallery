FROM node:15.14-alpine

WORKDIR /app

EXPOSE 3000

COPY --chown=node:node package.json package-lock.json ./

RUN npm install --silent

COPY --chown=node:node . ./

USER node

CMD ["npm", "start"]
