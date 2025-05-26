# Use Node.js LTS
FROM node:14

# Create app directory
WORKDIR /app

# Install dependencies
COPY package*.json ./
RUN npm install

# Copy the rest of the code
COPY . .

# Expose the port used by server.js
EXPOSE 3000

# Start the API server
CMD ["node", "server.js"]
