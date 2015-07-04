FROM alpine:3.2

#ENV S6_BEHAVIOUR_IF_STAGE2_FAILS=1

# Install redis
RUN apk add --update redis && \
    rm -rf /var/cache/apk/* && \
    mkdir /data && \
    chown -R redis:redis /data

# Add the files
COPY etc /etc/
WORKDIR /data
