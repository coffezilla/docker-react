# This image run reactjs and node for development
# all files are storage in the container
#

FROM node:14

WORKDIR /app

COPY package.json /app/package.json

RUN npm install

# add `/app/node_modules/.bin` to the $PATH
ENV PATH /app/node_modules/.bin:$PATH

COPY . .

# install react-script 
RUN npm install -g react-scripts
