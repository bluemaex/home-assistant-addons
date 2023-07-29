# bluemaex's Add-ons Shack

This repository contains my personal, but free to use [Home Assistant Add-ons](https://www.home-assistant.io/addons/).

[![Open your Home Assistant instance and show the add add-on repository dialog with a specific repository URL pre-filled.](https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg)](https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A%2F%2Fgithub.com%2Fbluemaex%2Fhome-assistant-addons)

## Usage

1. Navigate in your Home Assistant frontend to **Supervisor -> Add-on Store**
2. Add this new repository by URL (`https://github.com/bluemaex/home-assistant-addons`)
3. Find the add-on that you want to use and click it
4. Click on the "INSTALL" button

## Add-ons

This repository contains the following add-ons

### [rclone](./rclone)

Rclone as a backup tool for your backups and/or configuration.

### [traefik](./traefik)

Alternative way to expose Home Assistant and it's addons via automated HTTPS

### [VictoriaMetrics](./victoriametrics)

Time Series Database Database/Agent for long term storage

### [UnPoller](./unpoller)

Collect your UniFi controller data and report it to an InfluxDB instance, or export it for Prometheus collection.

### [Loki](./loki)

Grafana Loki is a horizontally-scalable, highly-available, multi-tenant log aggregation system inspired by Prometheus

### [promtail](./promtail)

Promtail is an agent which ships the contents of local logs to a private Loki instance or Grafana Cloud.

### [syslog-ng](./syslog-ng)

syslog-ng allows you to flexibly collect, parse, classify, rewrite and correlate logs from across your infrastructure and store or route them to log analysis tools

### [healtchecks](./healthchecks)

Healthchecks is a watchdog for your cron jobs. It's a web server that listens for pings from your cron jobs, plus a web interface.