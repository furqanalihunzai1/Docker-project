FROM golang:1.13-alpine
WORKDIR /app
COPY . .
EXPOSE 8000
ENTRYPOINT [ "go", "run", "http-server.go" ]