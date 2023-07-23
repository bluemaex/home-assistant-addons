ARG BUILD_FROM

FROM grafana/loki:2.8.3 as loki-base
FROM ${BUILD_FROM} AS final

COPY rootfs /
COPY --from=loki-base /usr/bin/loki /usr/bin/loki

RUN apk add --no-cache gomplate

# See https://github.com/grafana/loki/issues/1928
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf

RUN adduser -g "loki" --home /data/loki --disabled-password loki
