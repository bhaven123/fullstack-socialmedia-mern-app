# Base image
FROM node:lts

# Install nodemon
RUN npm install -g nodemon

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install 

# Copy the rest of the application code
COPY . .

# Expose the port on which the server will listen
EXPOSE 3001

# Start the server using nodemon with ECMAScript modules
CMD ["npm", "run", "start" ]