FROM alpine
RUN apk add --no-cache curl wget busybox-extras netcat-openbsd python3 py3-pip bash postgresql-client && \
    pip install awscli
RUN apk --purge -v del py3-pip
CMD tail -f /dev/null

