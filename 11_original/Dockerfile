FROM golang:latest

COPY main.go /go/src/
RUN go build -o /go/src/main /go/src/main.go
EXPOSE 8080
CMD ["go", "run", "/go/src/main.go"]
