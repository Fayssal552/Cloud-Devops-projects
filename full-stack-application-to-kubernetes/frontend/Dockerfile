# Base image
FROM node

# Set working directory so that all subsequent command runs in this folder
WORKDIR /app/frontend

# Copy package json and install dependencies
COPY package*.json ./
RUN npm install

# Copy our app
COPY . .

# Expose port to access server
EXPOSE 3000

# Command to run our app
CMD [ "npm", "start" ]