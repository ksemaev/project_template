FROM ubuntu
RUN apt update && apt install -y mysql-client postgresql-client screen && apt-get clean && rm -rf /var/lib/apt/lists/* && mkdir -p /mnt/dump
CMD tail -f /dev/null