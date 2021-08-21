FROM alpine
RUN apk add --no-cache curl bash python3 py-pip
RUN pip install awscli
RUN apk --purge -v del py-pip
RUN apk --purge -v del curl
CMD tail -f /dev/null
