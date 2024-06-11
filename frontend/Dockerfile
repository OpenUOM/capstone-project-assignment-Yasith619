# Use the specific Node.js version
FROM node:14

# Set the working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install Angular CLI 10
RUN npm install -g @angular/cli@10

# Install project dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose the port the app runs on
EXPOSE 4200

# Command to run the app
CMD ["ng", "serve", "--host", "0.0.0.0"]