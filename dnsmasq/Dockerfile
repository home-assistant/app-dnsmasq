ARG BUILD_FROM=ghcr.io/home-assistant/base:3.23
FROM $BUILD_FROM

# Add env
ENV LANG C.UTF-8

# Setup base
RUN apk add --no-cache dnsmasq

# Copy data
COPY rootfs /

LABEL \
    org.opencontainers.image.title="Home Assistant App: Dnsmasq" \
    org.opencontainers.image.description="A simple DNS server" \
    org.opencontainers.image.source="https://github.com/home-assistant/app-dnsmasq" \
    org.opencontainers.image.licenses="Apache License 2.0"
