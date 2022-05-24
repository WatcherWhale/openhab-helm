# openHAB - Helm Chart

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 3.2.0](https://img.shields.io/badge/AppVersion-3.2.0-informational?style=flat-square)

A helm chart for deploying openhab.

**Homepage:** <https://github.com/WatcherWhale/openhab-helm>

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://library-charts.k8s-at-home.com | common | 4.4.2 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| env | object | See below | environment variables. |
| env.GROUP_ID | int | `9001` | Set the correct group id |
| env.TZ | string | `"UTC"` | Set the container timezone |
| env.USER_ID | int | `9001` | Set the correct user id |
| image.pullPolicy | string | `"IfNotPresent"` | image pull policy |
| image.repository | string | `"openhab/openhab"` | image repository |
| image.tag | string | `"3.2.0-alpine"` | image tag |
| ingress.main | object | See values.yaml | Enable and configure ingress settings for the chart under this key. |
| persistence | object | See values.yaml | Configure persistence settings for the chart under this key. |
| probes | object | See values.yaml | Configures the probes for the main Pod. |
| service | object | See values.yaml | Configures service settings for the chart. |

## Chart Maintainers

| Name | GitHub |
| ---- | ------ |
| Mathias Maes | [https://github.com/WatcherWhale](https://github.com/WatcherWhale)
