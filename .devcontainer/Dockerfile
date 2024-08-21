FROM rapidsai/devcontainers:24.06-cpp-gcc12-cuda12.4-ubuntu22.04

# Pick up apt caches from host
RUN apt update && apt install auto-apt-proxy -y && apt-get clean -y && rm -rf /var/lib/apt/lists/*

# Install debug tools
RUN apt update && apt install gdb -y && apt-get clean -y && rm -rf /var/lib/apt/lists/*
