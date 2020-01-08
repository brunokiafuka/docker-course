# Use an existing docker image as a base
## alpine version of an img is the smallest version of a image
FROM node:alpine

WORKDIR /usr/app

# Download and install dependency
COPY ./package.json ./
RUN npm install
COPY ./ ./

# Tell the image what to do when it starts a container
CMD [ "npm", "start" ]