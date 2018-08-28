FROM alpine

RUN apk add --no-cache rsyslog
RUN addgroup -g 1043 rsyslog && adduser -u 1043 -G rsyslog -s /bin/sh -D rsyslog


COPY rsyslogd.conf /etc/rsyslogd.conf

USER rsyslog
EXPOSE 8514/tcp 8514/udp

CMD ["rsyslogd", "-n", "-f", "/etc/rsyslogd.conf", "-i", "/tmp/rsyslog.pid"]