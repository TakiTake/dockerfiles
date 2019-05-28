FROM alpine:3.9
ARG KUSTOMIZE_VERSION
RUN apk add --no-cache --virtual curl ca-certificates openssl \
    && curl -LO https://github.com/kubernetes-sigs/kustomize/releases/download/v${KUSTOMIZE_VERSION}/kustomize_${KUSTOMIZE_VERSION}_linux_amd64 \
    && mv kustomize_${KUSTOMIZE_VERSION}_linux_amd64 /usr/local/bin/kustomize \
    && chmod +x /usr/local/bin/kustomize \
    && apk del curl
