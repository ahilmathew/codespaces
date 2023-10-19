# Use the official Codespaces image
FROM mcr.microsoft.com/vscode/devcontainers/universal:linux

# Install Java 11
RUN sudo apt-get update \
    && sudo apt-get install -y openjdk-11-jdk

# Install Python and pip
RUN sudo apt-get install -y python3 python3-pip

# Install Node.js and npm
RUN curl -sL https://deb.nodesource.com/setup_$(lsb_release -cs).x | sudo -E bash - \
    && sudo apt-get install -y nodejs

# Install Yarn
RUN sudo npm install -g yarn

# Install pnpm
RUN sudo npm install -g pnpm

# Install PostgreSQL
RUN sudo apt-get install -y postgresql

