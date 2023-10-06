FROM node:16-alpine

#Install tools required
RUN npm i -g @nestjs/cli typescript \
    && apk add  git

COPY package.json ./
COPY package-lock.json ./
COPY ./ ./
RUN npm i

EXPOSE 5000

CMD ["npm", "run", "start"]