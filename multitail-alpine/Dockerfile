FROM alpine:3.16.1

ENV LANG='en_US.UTF-8' LANGUAGE='en_US:en' LC_ALL='en_US.UTF-8'$

RUN apk update
RUN apk add multitail

ENV MT_LOGS "/var/log/*.log"

CMD /usr/bin/multitail -w -D -Q 1 $MT_LOGS
