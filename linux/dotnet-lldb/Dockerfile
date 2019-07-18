#https://github.com/dotnet/coreclr/blob/master/Documentation/building/linux-instructions.md 
FROM mcr.microsoft.com/dotnet/core/sdk:2.2-stretch

RUN apt-get update && apt-get install -y \
    cmake llvm-3.9 \
    clang-3.9 \
    lldb-3.9 \
    liblldb-3.9-dev \
    libunwind8 \
    libunwind8-dev \
    gettext \
    libicu-dev \
    liblttng-ust-dev \
    libcurl4-openssl-dev \
    libssl-dev \
    uuid-dev \
    libnuma-dev \
    libkrb5-dev

# Kick off a container just to wait debugger to attach and run the app
ENTRYPOINT ["/bin/bash", "-c", "sleep infinity"]