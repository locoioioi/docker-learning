FROM node 

# set the working directory in the container
WORKDIR /app

# copy the application code to working directory
# if I did not set WORKDIR, the commadn would be
# COPY . /app
COPY . ./

# execute neccessary commands to run the application
RUN npm install

# docummentation purpose: expose the port the application runs on (optional * recommended)
EXPOSE 80

# start the application
# it only runs when the container is started
CMD ["node", "server.js"]

