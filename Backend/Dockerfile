# Use official Node. js image as the base image
FROM node:14-alpine

# # Set the working directory in the container
# WORKDIR /app

# Copy package json and package-lock.json files to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy all files to the working directory
COPY . .

# # Build the React app for production
# RUN npm run build

# Expose port 5000 to the outside world
EXPOSE 5000

# Command to run the application
CMD ["node", "server.js"]