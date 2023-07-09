ARG BUILD_ARCH
ARG BUILD_NAME="UnPoller"

FROM ghcr.io/home-assistant/aarch64-base:3.18 AS amd64-base
FROM ghcr.io/home-assistant/aarch64-base:3.18 AS armv7-base
FROM ghcr.io/home-assistant/aarch64-base:3.18 AS i386-base
FROM ghcr.io/home-assistant/aarch64-base:3.18 AS aarch64-base

FROM ghcr.io/unpoller/unpoller:v2.7.14 as unpoller-base

FROM ${BUILD_ARCH}-base AS final
COPY rootfs /
COPY --from=unpoller-base /usr/bin/unpoller /usr/local/bin/unpoller
COPY --from=unpoller-base /etc/unpoller/up.conf /etc/unpoller/up.conf

RUN apk add --no-cache gomplate

LABEL \
  io.hass.name="$BUILD_NAME for $BUILD_ARCH" \
  io.hass.description="Home Assistant Unofficial Add-on: $BUILD_ARCH $BUILD_NAME image" \
  maintainer="bluemaex <homeassistant@blmx.de>" \
  org.opencontainers.image.title="$BUILD_NAME for $BUILD_ARCH" \
  org.opencontainers.image.description="Home Assistant Unofficial Add-on: $BUILD_ARCH $BUILD_NAME image" \
  org.opencontainers.image.vendor="bluemaex" \
  org.opencontainers.image.authors="bluemaex <homeassistant@blmx.de>" \
  org.opencontainers.image.url="https://github.com/bluemaex/home-assistant-addons/$BUILD_NAME" \
  org.opencontainers.image.source="https://github.com/bluemaex/home-assistant-addons/$BUILD_NAME" \
  org.opencontainers.image.documentation="https://github.com/bluemaex/home-assistant-addons/blob/master/$BUILD_NAME/README.md" \
  org.opencontainers.image.created=${BUILD_DATE} \
  org.opencontainers.image.revision=${BUILD_REF} \
  org.opencontainers.image.version=${BUILD_VERSION}
