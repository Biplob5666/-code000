FROM mcr.microsoft.com/vscode/devcontainers/base:ubuntu-22.04

# Set noninteractive mode to avoid prompts
ENV DEBIAN_FRONTEND=noninteractive

# Update and install basic Kali-like tools
RUN apt-get update && apt-get install -y \
    sudo curl wget git nano net-tools iputils-ping nmap \
    python3 python3-pip \
    metasploit-framework \
    sqlmap nikto dirb hydra \
    && apt-get clean && rm -rf /var/lib/apt/lists/*

# Set default user
USER vscode
