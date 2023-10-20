# Use the Microsoft Dev Containers base image
FROM mcr.microsoft.com/devcontainers/base:bullseye

# Install Java 11
RUN apt-get update && \
    apt-get install -y openjdk-11-jdk

# Install Python and pip
RUN apt-get install -y python3 python3-pip

# Install Node.js and npm
RUN curl -sL https://deb.nodesource.com/setup_14.x | bash - && \
    apt-get install -y nodejs

# Install Yarn
RUN npm install -g yarn

# Install pnpm
RUN npm install -g pnpm

# Install PostgreSQL
RUN apt-get install -y postgresql

# Install Zsh
RUN apt-get install -y zsh

# Set the default shell to Zsh
# RUN chsh -s /usr/bin/zsh codespace
RUN chsh -s /usr/bin/zsh root

# Switch back to non-root user
# USER codespace
