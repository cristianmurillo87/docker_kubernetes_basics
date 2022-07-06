# Image used as base (from dockerhub)
FROM node:12

# Set the working directory
WORKDIR /app

# Copy a file to the container's working directory
COPY package.json .

# Run a command in the container
RUN npm install

# Copy all the files in the current path to the container's working directory
COPY . .

# Set buildtime arguments
ARG DEFAULT_PORT=80

# Set environment variables (also valid ENV PORT 80)
ENV PORT $DEFAULT_PORT

# EXPOSE is only for documentation purposes
EXPOSE $PORT

# Run a command to initialize the server (NodeJS)
CMD ["npm", "start"]