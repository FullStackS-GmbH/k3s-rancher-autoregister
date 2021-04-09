FROM alpine:latest

RUN apk update \
 && apk add jq \
 && apk add curl \
 && apk add bash \
 && rm -rf /var/cache/apk/*

RUN curl -LO https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/linux/amd64/kubectl

RUN chmod u+x kubectl && mv kubectl /usr/bin/kubectl

