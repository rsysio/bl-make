FROM golang:1.17.5

WORKDIR /app

COPY hello.go /app/

RUN go build /app/hello.go

FROM ubuntu:latest

WORKDIR /app

COPY --from=0 /app/hello /app/hello

CMD ["/app/hello"]
