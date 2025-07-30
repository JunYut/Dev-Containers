FROM mcr.microsoft.com/devcontainers/cpp:ubuntu

RUN apt-get update && apt-get install -y \
    vim \
    tree \
    && rm -rf /var/lib/apt/lists/*

# Install fastfetch
RUN wget https://github.com/fastfetch-cli/fastfetch/releases/download/2.48.1/fastfetch-linux-amd64.deb && \
    dpkg -i fastfetch-linux-amd64.deb && \
    apt install -f && \
    rm fastfetch-linux-amd64.deb
