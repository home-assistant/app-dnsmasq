# Base image updated by Renovate, update versionCompatibility on Alpine base bump
ARG BUILD_FROM=ghcr.io/home-assistant/base:3.23-2026.11.0@sha256:4c0c177f1b5072661cca81b97a1abc9f05121e9f2f649cdfcce8d15715fd80ea
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
