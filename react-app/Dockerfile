# This image run reactjs and node for development
# all files are storage on host, the container is only used to run the app
#
# TIP 1: alpine version lightweight than node image
# TIP 2: run bash from the the node image:
# $ docker run -it --entrypoint /bin/bash npm_app

FROM node:13-alpine

WORKDIR /app

# add `/app/node_modules/.bin` to the $PATH
ENV PATH /app/node_modules/.bin:$PATH

# install react-script 
RUN npm install -g react-scripts

CMD ["npm", "start"]
