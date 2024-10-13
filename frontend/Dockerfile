# Use an official Node.js image as the base
FROM node:16-alpine

# Set the working directory inside the container
WORKDIR /usr/src/app

# Copy the package.json and package-lock.json files
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the frontend source code
COPY . .

# Build the frontend app (for production)
RUN npm run build

# Expose port 3000 for the frontend
EXPOSE 3000

# Start the app
CMD ["npm", "start"]
