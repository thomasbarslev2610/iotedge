FROM alpine:3.10

RUN addgroup -S proxy && adduser -S proxy -G proxy
USER proxy

WORKDIR /app
COPY ./docker/linux/amd64/iotedge-proxy /app/iotedge-proxy

CMD ["/app/iotedge-proxy"]
