# Use the official Node.js 21 image from Docker Hub
FROM node:21-alpine

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json (if available) to the working directory
COPY package.json package-lock.json ./

# Install any needed packages specified in package.json
RUN npm install

# Copy the rest of the application code to the working directory
COPY . .

# Make port 8000 available to the world outside this container
EXPOSE 8000

# Define the command to run your app using CMD which keeps the container running
CMD ["node", "server.js"]
