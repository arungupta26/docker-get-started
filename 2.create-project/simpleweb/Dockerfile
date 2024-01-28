# specify a base image
# FROM alpine
FROM node:14-alpine

# set working directory

WORKDIR ./simpleweb

# copy local file system to docker container file system
COPY ./package.json ./

# install some dependencies
RUN npm install

# to avoid re run of npm install 
COPY ./ ./

# Default command

CMD ["npm", "start"]