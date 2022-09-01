FROM golang:1.19.0-bullseye

WORKDIR /app

RUN apt update

COPY . .

RUN go mod download

RUN go build main.go

EXPOSE 8080

CMD ["/main"]
