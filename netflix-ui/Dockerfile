# Use an official Node.js runtime as the base image
FROM node:18

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Build the React app
RUN npm run build

# Install 'serve' to serve the production build
RUN npm install -g serve

# Expose the app's port
EXPOSE 3000

# Start the React app
CMD ["serve", "-s", "build", "-l", "3000"]
