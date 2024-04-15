FROM node:16-alpine

WORKDIR /app

COPY package.json package-lock.json ./

RUN npm install

COPY . .

ENV POSTGRES_DB=express
ENV POSTGRES_HOST=db
ENV POSTGRES_USER=admin
ENV POSTGRES_PASSWORD=example
ENV ERASE_DATABASE_ON_SYNC=false

EXPOSE 3000

CMD ["npm", "start"]
