FROM node

WORKDIR /app

COPY package.json /app

RUN npm install

COPY . /app

ARG DEFAULT_PORT=80

ENV PORT $DEFAULT_PORT

EXPOSE $PORT

# anonymous volume ( managed by Docker )
# VOLUME [ "/app/feedback" ]

# named volume ( managed by programmer )
# docker run -d -p 3000:80 --rm --name feedback-app -v feedback:/app/feedback feedbackform:volumes

# Create a bind mount volume
# docker run -d -p 3000:80 --rm --name feedback-app -v feedback:/app/feedback -v "C:\work_space\docker-learning\day 2\1:/app" feedbackform:volumes

CMD [ "npm", "start" ]