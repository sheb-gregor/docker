# NAME:    shebgregor/ci-golang
FROM golang:1.11

LABEL maintainer "Michael Popsuev <sheb.gregor@gmail.com>"

RUN apt-get update &&\
    apt-get install -y rsync curl git && \
    go get -u github.com/golang/dep/cmd/dep