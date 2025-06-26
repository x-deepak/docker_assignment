FROM golang:1.22 AS builder
WORKDIR /app
COPY . .
RUN go build -o service_1 main.go

FROM gcr.io/distroless/base
COPY --from=builder /app/service_1 .
CMD ["/service_1"]
EXPOSE 8001