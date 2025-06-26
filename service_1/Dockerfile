FROM golang:1.22

WORKDIR /app

RUN apt-get update && apt-get install -y curl

COPY . .

EXPOSE 8001

CMD ["go", "run", "main.go"]