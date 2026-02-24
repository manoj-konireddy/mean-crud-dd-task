# Use lightweight Node.js image
FROM node:18-alpine

# Create app directory inside container
WORKDIR /app

# Copy package files first (best practice)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy rest of the backend code
COPY . .

# Expose backend port
EXPOSE 5000

# Start backend server
CMD ["npm", "start"]