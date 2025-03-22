# 1. Use an official Node.js image as a base image
FROM node:18-alpine

# 2. Set the working directory inside the container
WORKDIR /app

# 3. Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# 4. Install dependencies (npm install)
RUN npm install

# 5. Copy the rest of your application code into the container
COPY . .

# 6. Expose the port the app will run on
EXPOSE 3002

# 7. Define the command to run the application
CMD ["node", "app.js"]