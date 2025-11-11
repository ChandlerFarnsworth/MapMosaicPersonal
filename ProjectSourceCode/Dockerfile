# Use the official Node.js image
FROM node:18

# Set working directory inside container
WORKDIR /usr/src/app

# Copy package.json and lockfile (they're in the current directory now)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code (current directory)
COPY . .

# Expose the port your app listens on
EXPOSE 5000

# Start the app
CMD ["npm", "start"]