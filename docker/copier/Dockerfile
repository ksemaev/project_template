FROM alpine
RUN apk add rsync && mkdir -p /mnt/source && mkdir /mnt/destination
COPY rsyncd.conf /etc/rsyncd.conf
CMD tail -f /dev/null