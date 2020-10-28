FROM golang:1.14.10-alpine

ENV PATH /usr/local/go/bin:$PATH

ENV GOLANG_VERSION 1.14.10

RUN apk update && apk add make openssh-client zip && rm -rf /var/lib/apt/lists/*

ENV GOPATH /go
ENV PATH $GOPATH/bin:$PATH
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
WORKDIR $GOPATH
