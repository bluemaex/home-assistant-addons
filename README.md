# bluemaex's Add-ons Shack

![Project Stage][project-stage-shield]
![Maintenance][maintenance-shield]
[![License][license-shield]](LICENSE.md)

## About

Home Assistant allows anyone to create add-on repositories to share their
add-ons for Home Assistant easily. This repository contains my personal,
but free to use [Home Assistant Add-ons][ha-addons].

[![Add Repository Link][add-repository-image]][add-repository-button]

## Usage

Adding this add-ons repository to your Home Assistant instance is pretty
straightforward. In the Home Assistant add-on store, a possibility to
add a repository is provided.

1. Navigate in your Home Assistant frontend to **Supervisor -> Add-on Store**
1. Add this new repository by URL (`https://github.com/bluemaex/home-assistant-addons`)
1. Find the add-on that you want to use and click it
1. Click on the "INSTALL" button

## Add-ons

This repository contains the following add-ons:

### &#10003; [Grafana Loki][addon-grafana-loki]

![Latest Version][grafana-loki-version-shield]
![Supports armhf Architecture][grafana-loki-armhf-shield]
![Supports armv7 Architecture][grafana-loki-armv7-shield]
![Supports aarch64 Architecture][grafana-loki-aarch64-shield]
![Supports amd64 Architecture][grafana-loki-amd64-shield]

Grafana Loki is a horizontally-scalable, highly-available, multi-tenant log aggregation system inspired by Prometheus

[:books: Grafana Loki add-on documentation][addon-doc-grafana-loki]

### &#10003; [Grafana Promtail][addon-grafana-promtail]

![Latest Version][grafana-promtail-version-shield]
![Supports armhf Architecture][grafana-promtail-armhf-shield]
![Supports armv7 Architecture][grafana-promtail-armv7-shield]
![Supports aarch64 Architecture][grafana-promtail-aarch64-shield]
![Supports amd64 Architecture][grafana-promtail-amd64-shield]

Promtail is an agent which ships the contents of local logs to a private Loki instance or Grafana Cloud.

[:books: Grafana Promtail add-on documentation][addon-doc-grafana-promtail]

### &#10003; [healthchecks][addon-healthchecks]

![Latest Version][healthchecks-version-shield]
![Supports armhf Architecture][healthchecks-armhf-shield]
![Supports armv7 Architecture][healthchecks-armv7-shield]
![Supports aarch64 Architecture][healthchecks-aarch64-shield]
![Supports amd64 Architecture][healthchecks-amd64-shield]

Healthchecks is a watchdog for your cron jobs.
It's a web server that listens for pings from your cron jobs, plus a web interface.

[:books: healthchecks add-on documentation][addon-doc-healthchecks]

### &#10003; [Rclone][addon-rclone]

![Latest Version][rclone-version-shield]
![Supports armhf Architecture][rclone-armhf-shield]
![Supports armv7 Architecture][rclone-armv7-shield]
![Supports aarch64 Architecture][rclone-aarch64-shield]
![Supports amd64 Architecture][rclone-amd64-shield]

Rclone is a command line program to sync files and directories to and
from various providers.

[:books: Rclone add-on documentation][addon-doc-rclone]

### &#10003; [syslog-ng][addon-syslog-ng]

![Latest Version][syslog-ng-version-shield]
![Supports armhf Architecture][syslog-ng-armhf-shield]
![Supports armv7 Architecture][syslog-ng-armv7-shield]
![Supports aarch64 Architecture][syslog-ng-aarch64-shield]
![Supports amd64 Architecture][syslog-ng-amd64-shield]

syslog-ng allows you to flexibly collect, parse, classify, rewrite
and correlate logs from across your infrastructure and store or route
them to log analysis tools

[:books: syslog-ng add-on documentation][addon-doc-syslog-ng]

### &#10003; [Traefik][addon-traefik]

![Latest Version][traefik-version-shield]
![Supports armhf Architecture][traefik-armhf-shield]
![Supports armv7 Architecture][traefik-armv7-shield]
![Supports aarch64 Architecture][traefik-aarch64-shield]
![Supports amd64 Architecture][traefik-amd64-shield]

Traefik is a modern HTTP reverse proxy and load balancer that makes deploying
microservices easy.

[:books: Traefik add-on documentation][addon-doc-traefik]

### &#10003; [UnPoller][addon-unpoller]

![Latest Version][unpoller-version-shield]
![Supports armhf Architecture][unpoller-armhf-shield]
![Supports armv7 Architecture][unpoller-armv7-shield]
![Supports aarch64 Architecture][unpoller-aarch64-shield]
![Supports amd64 Architecture][unpoller-amd64-shield]

Collect your UniFi controller data and report it to an InfluxDB instance, or export it for Prometheus collection.

[:books: UnPoller add-on documentation][addon-doc-unpoller]

### &#10003; [Victoria Metrics][addon-victoriametrics]

![Latest Version][victoriametrics-version-shield]
![Supports armhf Architecture][victoriametrics-armhf-shield]
![Supports armv7 Architecture][victoriametrics-armv7-shield]
![Supports aarch64 Architecture][victoriametrics-aarch64-shield]
![Supports amd64 Architecture][victoriametrics-amd64-shield]

VictoriaMetrics is a fast, cost-effective and scalable monitoring solution and time series database.

[:books: Victoria Metrics add-on documentation][addon-doc-victoriametrics]


## License

MIT License

Copyright (c) 2023 Max Stockner

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

[add-repository-button]: https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https://github.com/bluemaex/home-assistant-addons
[ha-addons]: https://www.home-assistant.io/addons/
[add-repository-image]: https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg
[license-shield]: https://img.shields.io/github/license/bluemaex/home-assistant-addons.svg
[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
[project-stage-shield]: https://img.shields.io/badge/project%20stage-production%20ready-brightgreen.svg
[addon-grafana-loki]: https://github.com/bluemaex/home-assistant-addons/tree/grafana-loki-4.0.0
[addon-doc-grafana-loki]: https://github.com/bluemaex/home-assistant-addons/blob/grafana-loki-4.0.0/README.md
[grafana-loki-version-shield]: https://img.shields.io/badge/version-4.0.0-blue.svg
[grafana-loki-aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[grafana-loki-amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[grafana-loki-armhf-shield]: https://img.shields.io/badge/armhf-no-red.svg
[grafana-loki-armv7-shield]: https://img.shields.io/badge/armv7-no-red.svg
[addon-grafana-promtail]: https://github.com/bluemaex/home-assistant-addons/tree/grafana-promtail-4.0.0
[addon-doc-grafana-promtail]: https://github.com/bluemaex/home-assistant-addons/blob/grafana-promtail-4.0.0/README.md
[grafana-promtail-version-shield]: https://img.shields.io/badge/version-4.0.0-blue.svg
[grafana-promtail-aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[grafana-promtail-amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[grafana-promtail-armhf-shield]: https://img.shields.io/badge/armhf-no-red.svg
[grafana-promtail-armv7-shield]: https://img.shields.io/badge/armv7-no-red.svg
[addon-healthchecks]: https://github.com/bluemaex/home-assistant-addons/tree/healthchecks-3.1.3
[addon-doc-healthchecks]: https://github.com/bluemaex/home-assistant-addons/blob/healthchecks-3.1.3/README.md
[healthchecks-version-shield]: https://img.shields.io/badge/version-3.1.3-blue.svg
[healthchecks-aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[healthchecks-amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[healthchecks-armhf-shield]: https://img.shields.io/badge/armhf-no-red.svg
[healthchecks-armv7-shield]: https://img.shields.io/badge/armv7-no-red.svg
[addon-rclone]: https://github.com/bluemaex/home-assistant-addons/tree/rclone-3.1.6
[addon-doc-rclone]: https://github.com/bluemaex/home-assistant-addons/blob/rclone-3.1.6/README.md
[rclone-version-shield]: https://img.shields.io/badge/version-3.1.6-blue.svg
[rclone-aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[rclone-amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[rclone-armhf-shield]: https://img.shields.io/badge/armhf-no-red.svg
[rclone-armv7-shield]: https://img.shields.io/badge/armv7-yes-green.svg
[addon-syslog-ng]: https://github.com/bluemaex/home-assistant-addons/tree/syslog-ng-5.0.5
[addon-doc-syslog-ng]: https://github.com/bluemaex/home-assistant-addons/blob/syslog-ng-5.0.5/README.md
[syslog-ng-version-shield]: https://img.shields.io/badge/version-5.0.5-blue.svg
[syslog-ng-aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[syslog-ng-amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[syslog-ng-armhf-shield]: https://img.shields.io/badge/armhf-no-red.svg
[syslog-ng-armv7-shield]: https://img.shields.io/badge/armv7-no-red.svg
[addon-traefik]: https://github.com/bluemaex/home-assistant-addons/tree/traefik-4.2.6
[addon-doc-traefik]: https://github.com/bluemaex/home-assistant-addons/blob/traefik-4.2.6/README.md
[traefik-version-shield]: https://img.shields.io/badge/version-4.2.6-blue.svg
[traefik-aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[traefik-amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[traefik-armhf-shield]: https://img.shields.io/badge/armhf-no-red.svg
[traefik-armv7-shield]: https://img.shields.io/badge/armv7-yes-green.svg
[addon-unpoller]: https://github.com/bluemaex/home-assistant-addons/tree/unpoller-3.0.12
[addon-doc-unpoller]: https://github.com/bluemaex/home-assistant-addons/blob/unpoller-3.0.12/README.md
[unpoller-version-shield]: https://img.shields.io/badge/version-3.0.12-blue.svg
[unpoller-aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[unpoller-amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[unpoller-armhf-shield]: https://img.shields.io/badge/armhf-no-red.svg
[unpoller-armv7-shield]: https://img.shields.io/badge/armv7-yes-green.svg
[addon-victoriametrics]: https://github.com/bluemaex/home-assistant-addons/tree/victoriametrics-2.0.6
[addon-doc-victoriametrics]: https://github.com/bluemaex/home-assistant-addons/blob/victoriametrics-2.0.6/README.md
[victoriametrics-version-shield]: https://img.shields.io/badge/version-2.0.6-blue.svg
[victoriametrics-aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[victoriametrics-amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[victoriametrics-armhf-shield]: https://img.shields.io/badge/armhf-no-red.svg
[victoriametrics-armv7-shield]: https://img.shields.io/badge/armv7-yes-green.svg
