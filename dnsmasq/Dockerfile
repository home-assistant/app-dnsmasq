# Base image updated by Renovate, update versionCompatibility on Alpine base bump
ARG BUILD_FROM=ghcr.io/home-assistant/base:3.24-2026.11.1@sha256:5021aac8a4b7f2a1397e23a9749dfe9f736463ffa471df6b200216c68d530fe6
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
