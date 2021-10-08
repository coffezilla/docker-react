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