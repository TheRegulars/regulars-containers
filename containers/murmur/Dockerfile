FROM alpine:3.8

RUN apk --no-cache add murmur && mkdir -p /var/lib/murmur && mkdir -p /etc/murmur
VOLUME ["/var/lib/murmur", "/etc/murmur"]

USER murmur
ENTRYPOINT ["/usr/bin/murmurd", "-fg", "-ini", "/etc/murmur/mumble-server.ini"]
