# Define base image
FROM node:14.15.0-alpine3.12

# Specify home directory in container
WORKDIR /usr/src/app

# Copy file from local source location to a destination in container
COPY /src/ /usr/src/app/

# Download dependencies
RUN npm install

# Expose port
EXPOSE 8080

# Start command
CMD [ "node", "ratings.js", "8080" ]