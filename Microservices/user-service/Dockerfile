#Using slim version for smaller docker image
FROM node:16-slim

# Set the working directoryr
WORKDIR /app

# Copy package.jsone
COPY package*.json ./

#Installdependencies
RUN npm install --production

# Copy  the necessary application files 
COPY . .

# Exposing the port 3000
EXPOSE 3000

# Command to run the app
CMD ["node", "app.js"]
