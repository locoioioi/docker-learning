FROM node

WORKDIR /app

COPY package.json /app

RUN npm install

COPY . /app

ENV MONGODB_USERNAME=admin
ENV MONGODB_PASSWORD=admin

EXPOSE 80

CMD [ "npm", "start" ]