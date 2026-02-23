# Stage 1: Build
FROM node:25-alpine

# Set working directory
WORKDIR /app

# Copy package files and install dependencies
COPY package*.json ./
RUN npm install

# Copy the rest of the application
COPY . .

# Expose the backend port
EXPOSE 8080

# Start the server
CMD ["node", "server.js"]
