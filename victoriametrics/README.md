# Unofficial Home Assistant Add-ons: Victoria Metrics

Victoria Metrics (https://github.com/VictoriaMetrics/VictoriaMetrics) bundled as an Home Assistant add-on.

![aarch64-shield](https://img.shields.io/badge/aarch64-yes-green)
![amd64-shield](https://img.shields.io/badge/amd64-yes-green)
![armhf-shield](https://img.shields.io/badge/armhf-yes-green)
![armv7-shield](https://img.shields.io/badge/armv7-yes-green)

## About

VictoriaMetrics is a fast, cost-effective and scalable monitoring solution and time series database. It's a great choice if you want long term storage for your HomeAssistant Data and do custom evaluations longer than your default HomeAssistant Retention.

You can run this addon in two different ways:

### Server

Run an full [ultra efficent Time Series Database](https://github.com/VictoriaMetrics/VictoriaMetrics#prominent-features) Server even on low speced computers as the Raspberry PI.

### Agent

This add-on makes it easy to scrape (i.e. fetch) metrics locally, cache them in a local temporary database, and send them to your centralized Victoria Metrics Time Series Database Server as soon as is is reachable, thus allowing to have full data even if the database is down or unreachable at times.

## Final notes

For information on how to configure this addon please refer to the [Documentation](DOCS.md) inside the addon page

This project is not affiliated with Victoria Metrics, the Victoria Metrics Maintainer Team, but simply a community effort. Victoria Metrics itself is distributed under the [Apache License 2.0](https://github.com/VictoriaMetrics/VictoriaMetrics/blob/master/LICENSE).
