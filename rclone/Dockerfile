ARG BUILD_ARCH

FROM ghcr.io/home-assistant/aarch64-base:3.18 AS aarch64-base
FROM ghcr.io/home-assistant/amd64-base:3.18 AS amd64-base
FROM ghcr.io/home-assistant/armv7-base:3.16 AS armv7-base
FROM ghcr.io/home-assistant/armhf-base:3.16 AS armhf-base
FROM ghcr.io/home-assistant/i386-base:3.18 AS i386-base
FROM rclone/rclone:1.61.1 as rclone-base

FROM ${BUILD_ARCH}-base AS final
COPY rootfs /
COPY --from=rclone-base /usr/local/bin/rclone /usr/local/bin/rclone

LABEL \
  io.hass.name="Rclone for ${BUILD_ARCH}" \
  io.hass.description="Home Assistant Unofficial Add-on: ${BUILD_ARCH} Rclone image" \
  maintainer="bluemaex <homeassistant@blmx.de>" \
  org.opencontainers.image.title="Rclone for ${BUILD_ARCH}" \
  org.opencontainers.image.description="Home Assistant Unofficial Add-on: ${BUILD_ARCH} Rclone image" \
  org.opencontainers.image.vendor="bluemaex" \
  org.opencontainers.image.authors="bluemaex <homeassistant@blmx.de>" \
  org.opencontainers.image.url="https://github.com/bluemaex/home-assistant-addons/" \
  org.opencontainers.image.source="https://github.com/bluemaex/home-assistant-addons/" \
  org.opencontainers.image.documentation="https://github.com/bluemaex/home-assistant-addons/blob/master/rclone/README.md" \
  org.opencontainers.image.created=${BUILD_DATE} \
  org.opencontainers.image.revision=${BUILD_REF} \
  org.opencontainers.image.version=${BUILD_VERSION}
