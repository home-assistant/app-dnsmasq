# Base image updated by Renovate, update versionCompatibility on Alpine base bump
ARG BUILD_FROM=ghcr.io/home-assistant/base:3.24-2026.11.0@sha256:58422480a299b16b6ea376c2167463206d430619ed02b40cd687c8bd6875519e
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
