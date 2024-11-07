# Dockerfile
# Use a lightweight base image
FROM alpine:latest

# Set the working directory in the container
WORKDIR /app

# Copy the rest of the application code into the container
COPY . .

# Install necessary packages
RUN apk update && apk add curl

# Define a simple entrypoint
CMD ["echo", "Hello from the Docker container!"]

