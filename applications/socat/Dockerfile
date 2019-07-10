FROM alpine:latest
#USER root
#Installing socat

RUN rm -rf /var/cache/apk/* && \
    rm -rf /tmp/*
RUN apk update

RUN apk update && apk upgrade && apk add bash socat
COPY entrypoint.sh entrypoint.sh
ENTRYPOINT ["sh", "./entrypoint.sh"]
