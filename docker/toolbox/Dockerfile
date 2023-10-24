FROM alpine
RUN apk add --no-cache curl wget busybox-extras netcat-openbsd python3 py3-pip bash && \
    pip install awscli
RUN apk --purge -v del py3-pip
CMD tail -f /dev/null

