# Base image
FROM node:16-alpine

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy server files
COPY . .

# Expose the port
EXPOSE 5000

# Set the entrypoint command
CMD [ "node", "index.js" ]
