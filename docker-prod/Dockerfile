FROM alpine:latest

RUN apk update && \
    apk add ca-certificates git bash python py-pip jq && \
    pip install awscli && \
    apk --purge -v del py-pip && \
    rm /var/cache/apk/*

COPY terraform/* /usr/local/bin/
COPY check in out /opt/resource/
