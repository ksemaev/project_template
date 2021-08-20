FROM alpine
RUN apk add --no-cache curl wget busybox-extras netcat-openbsd bash
RUN apk --purge -v del curl
CMD tail -f /dev/null
