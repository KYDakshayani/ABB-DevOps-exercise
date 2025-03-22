# Use the official Ubuntu image as a base image
FROM ubuntu:20.04

# Set environment variables to avoid interactive prompts during package installation
ENV DEBIAN_FRONTEND=noninteractive

# Update package list and install curl
RUN apt-get update && apt-get install -y curl

# Set the working directory
WORKDIR /app

# Create a simple "Hello, World!" script
RUN echo '#!/bin/bash \n echo "Hello, World!"' > /app/hello.sh && chmod +x /app/hello.sh

# Command to run when the container starts
CMD ["/app/hello.sh"]
