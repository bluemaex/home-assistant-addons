ARG BUILD_ARCH

FROM ghcr.io/home-assistant/aarch64-base:3.16 AS aarch64-base
FROM ghcr.io/home-assistant/amd64-base:3.16 AS amd64-base
FROM ghcr.io/home-assistant/armv7-base:3.16 AS armv7-base
FROM ghcr.io/home-assistant/armhf-base:3.16 AS armhf-base
FROM traefik:2.9.6 as traefik-base

FROM ${BUILD_ARCH}-base AS final
COPY rootfs /
COPY --from=traefik-base /usr/local/bin/traefik /usr/local/bin/traefik
RUN apk add --no-cache nginx gomplate

LABEL \
  io.hass.name="Treafik for ${BUILD_ARCH}" \
  io.hass.description="Home Assistant Unofficial Add-on: ${BUILD_ARCH} Treafik image" \
  maintainer="bluemaex <homeassistant@blmx.de>" \
  org.opencontainers.image.title="Traefik for ${BUILD_ARCH}" \
  org.opencontainers.image.description="Home Assistant Unofficial Add-on: ${BUILD_ARCH} Traefik image" \
  org.opencontainers.image.vendor="bluemaex" \
  org.opencontainers.image.authors="bluemaex <homeassistant@blmx.de>" \
  org.opencontainers.image.url="https://github.com/bluemaex/home-assistant-addons/traefik" \
  org.opencontainers.image.source="https://github.com/bluemaex/home-assistant-addons/traefik" \
  org.opencontainers.image.documentation="https://github.com/bluemaex/home-assistant-addons/blob/master/traefik/README.md" \
  org.opencontainers.image.created=${BUILD_DATE} \
  org.opencontainers.image.revision=${BUILD_REF} \
  org.opencontainers.image.version=${BUILD_VERSION}
