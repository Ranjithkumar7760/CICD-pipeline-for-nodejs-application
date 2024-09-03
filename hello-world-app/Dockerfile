# Use the official Node.js image.
FROM node:14-alpine

# Set the working directory.
WORKDIR /app

# Copy the package.json and package-lock.json files.
COPY package*.json ./

# Install dependencies.
RUN npm install

# Copy the rest of the application.
COPY . .

# Expose the port the app runs on.
EXPOSE 3000

# Define the command to run the application.
CMD ["node", "app.js"]
