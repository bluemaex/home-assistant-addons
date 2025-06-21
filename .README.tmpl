{{- $repo := .Env.REPOSITORY -}}
{{- $repo_url := .Env.REPOSITORY_URL -}}
{{- $arch := .Env.ARCHITECTURES | jsonArray -}}
{{- $addons := .Env.ADDONS_DATA | jsonArray -}}

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
1. Add this new repository by URL (`{{ $repo_url }}`)
1. Find the add-on that you want to use and click it
1. Click on the "INSTALL" button

## Add-ons

This repository contains the following add-ons:
{{ range $addons }}
### &#10003; [{{ .name }}][addon-{{ .slug }}]

![Latest Version][{{ .slug }}-version-shield]
![Supports armhf Architecture][{{ .slug }}-armhf-shield]
![Supports armv7 Architecture][{{ .slug }}-armv7-shield]
![Supports aarch64 Architecture][{{ .slug }}-aarch64-shield]
![Supports amd64 Architecture][{{ .slug }}-amd64-shield]

{{ .description }}
[:books: {{ .name }} add-on documentation][addon-doc-{{ .slug }}]
{{ end }}

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

[add-repository-button]: https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url={{ $repo_url }}
[ha-addons]: https://www.home-assistant.io/addons/
[add-repository-image]: https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg
[license-shield]: https://img.shields.io/github/license/{{ $repo }}.svg
[maintenance-shield]: https://img.shields.io/maintenance/yes/2025.svg
[project-stage-shield]: https://img.shields.io/badge/project%20stage-production%20ready-brightgreen.svg
{{- range $addons }}
[addon-{{ .slug }}]: {{ $repo_url }}/tree/{{.slug}}-{{ .version }}
[addon-doc-{{ .slug }}]: {{ $repo_url }}/blob/{{.slug}}-{{ .version }}/README.md
[{{ .slug }}-version-shield]: https://img.shields.io/badge/version-{{ .version | strings.ReplaceAll "-" "--" }}-blue.svg
{{- $addon := . }}
{{- range $arch }}
{{- if has $addon.arch . }}
[{{ $addon.slug }}-{{ . }}-shield]: https://img.shields.io/badge/{{ . }}-yes-green.svg
{{- else }}
[{{ $addon.slug }}-{{ . }}-shield]: https://img.shields.io/badge/{{ . }}-no-red.svg
{{- end }}
{{- end }}
{{- end }}
