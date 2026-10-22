ARG BUILD_FROM=ghcr.io/home-assistant/base:3.24

FROM ghcr.io/unpoller/unpoller:v5.7.0 AS unpoller-base
FROM ${BUILD_FROM} AS final

COPY rootfs /
COPY --from=unpoller-base /usr/bin/unpoller /usr/local/bin/unpoller
COPY --from=unpoller-base /etc/unpoller/up.conf /etc/unpoller/up.conf

RUN apk add --no-cache gomplate

LABEL \
    maintainer="bluemaex <homeassistant@blmx.de>" \
    org.opencontainers.image.authors="bluemaex <homeassistant@blmx.de>" \
    org.opencontainers.image.licenses="MIT License" \
    org.opencontainers.image.title="Home Assistant Unofficial Add-on: unpoller" \
    org.opencontainers.image.url="https://github.com/bluemaex/home-assistant-addons" \
    org.opencontainers.image.documentation="https://github.com/bluemaex/home-assistant-addons/unpoller/README.md"
