FROM alpine
RUN apk add --no-cache curl wget busybox-extras netcat-openbsd bash python3 py-pip
RUN pip install awscli
RUN aok --purge -v del py3-pip
RUN apk --purge -v del curl
CMD tail -f /dev/null
