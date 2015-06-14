FROM mhart/alpine-iojs:2.1.0
RUN apk add --update python make alpine-sdk && \
    rm /var/cache/apk/*
WORKDIR /src
COPY . /src/
RUN npm install
RUN npm install -g anvil-connect
RUN nv init
