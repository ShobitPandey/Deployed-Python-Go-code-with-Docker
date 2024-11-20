FROM golang:1.19
WORKDIR /app
COPY go.mod ./
RUN go mod download || true
COPY main.go .
RUN go build -o app .
CMD ["./app"]
