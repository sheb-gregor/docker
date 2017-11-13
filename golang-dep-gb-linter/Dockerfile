FROM golang:1.8.5-alpine3.6

MAINTAINER sheb.gregor@gmail.com<Michael Popsuev>

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
