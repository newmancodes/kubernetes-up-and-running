# Start from a Node.js 
FROM node:14.15.2

# Specify the directory inside the image in which all the commands wil lrun
WORKDIR /usr/src/app

# Copy package files and install dependencies
COPY package*.json ./
RUN npm ci

# Copy all of the app files into the image
COPY . .

# The default command to run when starting the container
CMD [ "npm", "start" ]