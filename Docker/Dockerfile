# build this image, from the specific image
FROM ubuntu:22.04

# copy files from host into container
# / at the end means that if the folder is no created, it will create it.
COPY src /app/

# Set the working directory (in container) for all commands & like changing into a directory - "cd"
WORKDIR /app

# This will be executed when docker container starts & only 1 "CMD" instruction in a Dockerfile
# [ command/executable, parameter ]
CMD ["bash", "my_run.sh"]
