FROM alpine:3.9
ARG KUBECTL_VERSION
RUN apk add --no-cache --virtual curl ca-certificates openssl \
    && curl -LO https://storage.googleapis.com/kubernetes-release/release/v${KUBECTL_VERSION}/bin/linux/amd64/kubectl \
    && mv kubectl /usr/local/bin/kubectl \
    && chmod +x /usr/local/bin/kubectl \
    && apk del curl
