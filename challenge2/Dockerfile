# Use an official Node.js runtime as a parent image
FROM node:latest

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json or yarn.lock if available
# Assuming you have package.json in the same directory as your server.js
COPY package*.json ./

# Install any dependencies
RUN npm install

# Bundle app source
COPY . .

# Set the environment variable PORT to 8080
ENV PORT=8080

# Expose port 8080 to the outside once the container is running
EXPOSE 8080

# Define the command to run your app using CMD
CMD ["node", "server.js"]
