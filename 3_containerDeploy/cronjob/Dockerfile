# cron jobを試す
# 1ジョブ1コンテナにしがちだけど、それは複雑になるからこんな感じで実現
FROM ubuntu:16.04

RUN apt update
RUN apt install -y cron

COPY task.sh /usr/local/bin/
COPY cron-example /etc/cron.d/
RUN chmod 0644 /etc/cron.d/cron-example

CMD ["cron", "-f"]
