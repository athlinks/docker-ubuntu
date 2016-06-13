FROM ubuntu:15.10

RUN DOCKERIZE_VERSION="0.2.0" && \
    DOCKERIZE_URL="https://github.com/jwilder/dockerize/releases/download/v$DOCKERIZE_VERSION" && \
    DOCKERIZE_PKG="dockerize-linux-amd64-v$DOCKERIZE_VERSION.tar.gz" && \
    apt-get update && \
    apt-get -y dist-upgrade && \
    apt-get install -y curl wget && \
    cd /tmp && \
    curl -L $DOCKERIZE_URL/$DOCKERIZE_PKG -o $DOCKERIZE_PKG && \
    tar -C /usr/local/bin -xzvf dockerize-linux-amd64-v$DOCKERIZE_VERSION.tar.gz && \
    rm -rf /tmp/* /var/lib/apt/lists/*
