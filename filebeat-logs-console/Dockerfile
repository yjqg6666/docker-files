FROM alpine:3.16.1

ENV LANG='en_US.UTF-8' LANGUAGE='en_US:en' LC_ALL='en_US.UTF-8'$

COPY ./edge-repositories /etc/apk/repositories

RUN apk update
RUN apk add filebeat

CMD ["/usr/bin/filebeat", "-c", "/etc/filebeat/filebeat.yml"]

COPY ./my-filebeat.yml /etc/filebeat/filebeat.yml
