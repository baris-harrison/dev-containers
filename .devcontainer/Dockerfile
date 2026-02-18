# Dockerfile
ARG PYTHON_VERSION=3.12

# Start from Microsoft's Python dev container base
FROM mcr.microsoft.com/devcontainers/python:${PYTHON_VERSION}
# Add source code
COPY . /app

# Change to app directory
WORKDIR /app

# Upgrade pip and install application including dependencies
RUN pip3 install -r requirements.txt