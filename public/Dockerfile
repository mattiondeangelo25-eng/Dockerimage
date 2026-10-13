# Use the official Node.js 16 base image from Docker Hub
FROM node:16

# Set the working directory inside the container for all subsequent commands
WORKDIR /usr/src/app

# Copy the package.json file from your host machine to the container's working directory
COPY package.json ./

# Install the application dependencies listed in package.json
RUN npm install

# Copy all the remaining application files from your host machine to the container
COPY . .

# Expose port 3000 to allow network traffic to the containerized application
EXPOSE 3000

# Start the application using the specified runtime command
CMD ["npm", "start"]
