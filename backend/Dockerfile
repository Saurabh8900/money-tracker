# Base image
FROM node:18

# Set working directory
WORKDIR /app

# Copy package.json and install dependencies
COPY package*.json ./
RUN npm install

# Copy rest of the backend files
COPY . .

# Expose the port your backend runs on
EXPOSE 5000

# Start the backend server
CMD ["npm", "run", "dev"]
