# Use Node base image
FROM node:18

# Set working directory inside container
WORKDIR /app

# Copy only package files first
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the app code
COPY . .

# Expose your backend port
EXPOSE 5000

# Start dev server (nodemon)
CMD ["npm", "run", "dev"]
