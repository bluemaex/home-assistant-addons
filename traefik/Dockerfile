ARG BUILD_FROM

FROM traefik:2.10.7 as traefik-base
FROM ${BUILD_FROM} AS final

COPY rootfs /
COPY --from=traefik-base /usr/local/bin/traefik /usr/local/bin/traefik
RUN apk add --no-cache nginx gomplate
