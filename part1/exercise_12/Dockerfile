# Dockerfile for starting the example-frontend

# Install Node version 16
FROM node:16

# expose port 5000
EXPOSE 5000

WORKDIR /usr/src/app

# Copy package.json and package-lock.json inside of the container
COPY package*.json ./

# Install all dependencies
RUN npm install
RUN npm install -g serve

# Copy all source code
COPY . . 

# add environment variables
ENV REACT_APP_BACKEND_URL="http://localhost:8080"

# build the static files
RUN npm run build

# Use npm package called serve to serve the project in port 5000
CMD ["serve", "-s", "-l", "5000", "build"]