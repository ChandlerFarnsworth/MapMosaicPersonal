# Use the official Node.js image
FROM node:18

# Set working directory inside container
WORKDIR /usr/src/app

# Copy package.json and lockfile from ProjectSourceCode
COPY ProjectSourceCode/package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY ProjectSourceCode/ ./

# Expose the port your app listens on
EXPOSE 5000

# Start the app
CMD ["npm", "start"]
