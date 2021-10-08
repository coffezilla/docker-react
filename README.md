# Docker React
This docker React example is used to create a container running node for React projects.
All the React content runs in the host side, the container is used only to run the application inside the node enviroment, so, this way you don't need to install node versions in the host.

## How to use
- After clone this repo, use the terminal and navigate to the 'react-app' folder
- Inside the 'react-app' folder, use 'npm install' to install all the dependencies
- Use 'docker-compose up' to start the container running your app

## Tips
- Edit .env file in order to change the name of the container and change the default (3000) port
- You need to change the CONTAINER_PREFIX and APP_PORT inside the .env file in order to create many containers

## How to use Docker with a React already created
To use this Dockerfile and docker-compose.yml in a project already created (using create-react-app), just copy the Dockerfile and docker-compose.yml and put them in the root of your react app.

After that, just call the 'docker-compose up' and it will just start the container for you.

## Why node alpine version?
The node tagged with alpine is lightweight than default node. the alpine is secure and has all you need to run a simple react app.

If you want to use the node default, it will be weight but it allow you to use bash:
**docker run -it --entrypoint /bin/bash my_node_image**
