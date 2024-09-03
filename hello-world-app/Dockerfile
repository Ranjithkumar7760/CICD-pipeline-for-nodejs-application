# Use the official Node.js image.
FROM node:14-alpine

# Set the working directory inside the container.
WORKDIR /app

# Copy the package.json and package-lock.json files to leverage Docker cache.
COPY package*.json ./

# Install dependencies.
RUN npm install

# Copy the rest of the application.
COPY . .

# Expose the port the app runs on.
EXPOSE 3000

# Command to run the application.
CMD ["node", "app.js"]
