# Use an official Node.js image as the base
FROM node:16-alpine

# Set the working directory
WORKDIR /usr/src/app

# Copy the package.json and install dependencies
COPY package*.json ./
RUN npm install

# Copy the backend source code
COPY . .

# Expose the API port
EXPOSE 5000

# Start the backend server
CMD ["node", "server.js"]
