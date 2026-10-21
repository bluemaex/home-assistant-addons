# Unofficial Home Assistant Add-ons: Terrastate

[Terrastate](https://github.com/webhippie/terrastate) bundled as a Home Assistant add-on.

## About

Terrastate is a small HTTP state backend for Terraform and OpenTofu. It
implements the native `http` backend protocol — including state locking — and
stores each workspace as a flat file on disk. Running it as a Home Assistant
add-on keeps your Terraform state on independent infrastructure with its own
backup lifecycle, decoupled from the machines it provisions.

## Final notes

For information on how to configure this addon please refer to the
[Documentation](DOCS.md) inside the addon page.

This project is not affiliated with Terrastate, but simply a community effort.
Terrastate itself is distributed under the Apache-2.0 license.
