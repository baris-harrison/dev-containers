# Dockerfile
ARG PYTHON_VERSION=3.12

# Start from Microsoft's Python dev container base
FROM mcr.microsoft.com/devcontainers/python:${PYTHON_VERSION}

LABEL org.opencontainers.image.source=https://github.com/baris-harrison/dev-container
LABEL org.opencontainers.image.description="Python 3.12 Dev Container for VS Code"
LABEL org.opencontainers.image.licenses=MIT
# Set working directory
WORKDIR /app

# Copy the requirements file into the container
COPY requirements.txt .

# Install the dependencies
RUN pip install --no-cache-dir -r requirements.txt

