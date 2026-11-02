# Base image updated by Renovate, update versionCompatibility on Alpine base bump
ARG BUILD_FROM=ghcr.io/home-assistant/base:3.23-2026.10.3@sha256:1550b137f45bbb61f932a5ec97265c1d8594ddc4a986b127fb06a5c8c4bcaa6d
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
