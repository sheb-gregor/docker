# NAME:    shebgregor/golang-dep-gb-linter
FROM rust:1.31

LABEL maintainer "Michael Popsuev <sheb.gregor@gmail.com>"

RUN apt-get update \
  && apt-get install -y autoconf automake libtool curl make g++ unzip libssl-dev pkg-config libsodium-dev librocksdb-dev 

ENV ROCKSDB_LIB_DIR=/usr/lib/x86_64-linux-gnu
ENV SNAPPY_LIB_DIR=/usr/lib/x86_64-linux-gnu

# INSTALL PROTOC
# Make sure you grab the latest version
RUN curl -OL https://github.com/google/protobuf/releases/download/v3.6.1/protoc-3.6.1-linux-x86_64.zip
# Unzip
RUN unzip protoc-3.6.1-linux-x86_64.zip -d protoc3
# Move protoc to /usr/local/bin/
RUN mv protoc3/bin/* /usr/local/bin/
# Move protoc3/include to /usr/local/include/
RUN mv protoc3/include/* /usr/local/include/
RUN protoc --version