# origin image
FROM node:13-alpine

WORKDIR /app

# add `/app/node_modules/.bin` to the $PATH
ENV PATH /app/node_modules/.bin:$PATH

COPY . .

# install react-script 
RUN npm install -g react-scripts

CMD ["npm", "start"]