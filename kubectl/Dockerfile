FROM alpine:3.9
ARG VERSION
RUN apk add --no-cache --virtual curl ca-certificates openssl \
    && curl -LO https://storage.googleapis.com/kubernetes-release/release/v${VERSION}/bin/linux/amd64/kubectl \
    && mv kubectl /usr/local/bin/kubectl \
    && chmod +x /usr/local/bin/kubectl \
    && apk del curl
