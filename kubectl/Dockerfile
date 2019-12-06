FROM alpine:3.10.3
ARG VERSION=1.16.3
RUN apk add --no-cache curl ca-certificates openssl \
    && curl -LO https://storage.googleapis.com/kubernetes-release/release/v${VERSION}/bin/linux/amd64/kubectl \
    && mv kubectl /usr/local/bin/kubectl \
    && chmod +x /usr/local/bin/kubectl \
    && apk del curl
