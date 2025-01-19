#Using slim version for smaller docker image
FROM node:16-slim

# Set the working directory
WORKDIR /app

# Copy package.json
COPY package*.json ./

#Installdependencies
RUN npm install --production

# Copy  the necessary application files 
COPY . .

# Exposing the port 3002
EXPOSE 3002

# Command to run the app
CMD ["node", "app.js"]
