# build this image, from the specific image
FROM node:20-alpine

# copy files from host into container
# / at the end means that if the folder is no created, it will create it.
COPY package.json /app/
COPY src /app/

# Set the working directory (in container) for all commands & like changing into a directory - "cd"
WORKDIR /app

# this will execute any command in a shell inside the container
RUN npm install

# This will be executed when docker container starts & only 1 "CMD" instruction in a Dockerfile
# [ command/executable, parameter ]
CMD ["node", "server.js"]