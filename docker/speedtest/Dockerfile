FROM alpine
RUN apk update && apk add bash  python3 py-pip && \
    pip install speedtest-cli
COPY run.sh /usr/bin/run.sh
RUN chmod +x /usr/bin/run.sh

ENTRYPOINT /usr/bin/run.sh
