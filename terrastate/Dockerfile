ARG BUILD_FROM

FROM webhippie/terrastate:2.11.0 AS terrastate-base
FROM ${BUILD_FROM} AS final

ARG USERNAME=terrastate

COPY rootfs /
COPY --from=terrastate-base /usr/bin/terrastate /usr/local/bin/terrastate

RUN apk add --no-cache gomplate \
    && addgroup "${USERNAME}" \
    && adduser -S -G "${USERNAME}" "${USERNAME}"
