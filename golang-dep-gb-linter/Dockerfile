# NAME:    shebgregor/golang-dep-gb-linter
FROM golang:1.11-alpine3.6

LABEL maintainer "Michael Popsuev <sheb.gregor@gmail.com>"

RUN true && \
    apk add --update  git python py-pip bash gcc libc-dev \
    ca-certificates bash curl rsync openssh && \
    pip install pre-commit && \
    go get -u github.com/constabulary/gb/... && \
    go install github.com/constabulary/gb && \
    go get -u github.com/golang/dep/cmd/dep && \
    go get -u github.com/alecthomas/gometalinter && \
    go get -u github.com/golang/lint/golint && \
    gometalinter --install 1> /dev/null
