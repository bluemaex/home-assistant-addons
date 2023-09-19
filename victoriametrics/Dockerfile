ARG BUILD_ARCH
ARG NAME="VictoriaMetrics"

FROM ghcr.io/home-assistant/aarch64-base:3.18 AS aarch64-base
FROM ghcr.io/home-assistant/amd64-base:3.18 AS amd64-base
FROM ghcr.io/home-assistant/armv7-base:3.18 AS armv7-base
FROM ghcr.io/home-assistant/i386-base:3.18 AS i386-base

FROM victoriametrics/victoria-metrics:v1.93.5 as victoriametrics-server
FROM victoriametrics/vmagent:v1.93.5 as victoriametrics-agent

FROM ${BUILD_ARCH}-base AS final
COPY rootfs /
COPY --from=victoriametrics-server /victoria-metrics-prod /usr/local/bin/victoria-metrics-prod
COPY --from=victoriametrics-agent /vmagent-prod /usr/local/bin/vmagent-prod

LABEL \
  io.hass.name="${NAME} for ${BUILD_ARCH}" \
  io.hass.description="Home Assistant Unofficial Add-on: ${BUILD_ARCH} ${NAME} image" \
  maintainer="bluemaex <homeassistant@blmx.de>" \
  org.opencontainers.image.title="${NAME} for ${BUILD_ARCH}" \
  org.opencontainers.image.description="Home Assistant Unofficial Add-on: ${BUILD_ARCH} ${NAME} image" \
  org.opencontainers.image.vendor="bluemaex" \
  org.opencontainers.image.authors="bluemaex <homeassistant@blmx.de>" \
  org.opencontainers.image.url="https://github.com/bluemaex/home-assistant-addons/${NAME}" \
  org.opencontainers.image.source="https://github.com/bluemaex/home-assistant-addons/${NAME}" \
  org.opencontainers.image.documentation="https://github.com/bluemaex/home-assistant-addons/blob/master/${NAME}/README.md" \
  org.opencontainers.image.created=${BUILD_DATE} \
  org.opencontainers.image.revision=${BUILD_REF} \
  org.opencontainers.image.version=${BUILD_VERSION}
