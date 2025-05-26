# Use Node.js LTS
FROM node:14

# Create app directory
WORKDIR /app

# Install dependencies
COPY package*.json ./
RUN npm install

# Copy source code
COPY . .

# Expose frontend port (React default is 3000)
EXPOSE 3000

# Start React app
CMD ["npm", "start"]
