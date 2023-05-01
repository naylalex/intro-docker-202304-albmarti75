FROM golang:1.20 as build

RUN mkdir /web
WORKDIR /web
COPY dispatcher.go .
RUN go build dispatcher.go
