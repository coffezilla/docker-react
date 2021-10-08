# This image run reactjs and install all node_modules inside the local package.json
# the node_modules can be storaged inside the container or local in the host
#
# TIP: run bash from the the image:
# docker run -it --entrypoint /bin/bash npm_app

# origin image
FROM node:13-alpine

WORKDIR /app

# add `/app/node_modules/.bin` to the $PATH
ENV PATH /app/node_modules/.bin:$PATH

COPY . .

# update packages
RUN apt-get update
RUN npm install

# install react-script 
RUN npm install -g react-scripts

CMD ["npm", "start"]