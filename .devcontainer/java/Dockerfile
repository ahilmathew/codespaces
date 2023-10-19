# Use the official Codespaces image
FROM mcr.microsoft.com/devcontainers/base:alpine

# Install Java 11
RUN apk add --no-cache openjdk11

# Install Python and pip
RUN apk add --no-cache python3 py3-pip

# Install Node.js and npm
RUN apk add --no-cache nodejs npm

# Install Yarn
RUN npm install -g yarn

# Install pnpm
RUN npm install -g pnpm

# Install PostgreSQL
RUN apk add --no-cache postgresql

# Switch back to non-root user
# USER vscode