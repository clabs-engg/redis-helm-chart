# [`helm`-charts](https://charts.pascaliske.dev)

> Another repository with lightweight Helm Charts.

[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/pascaliske&style=flat-square)](https://artifacthub.io/packages/search?repo=pascaliske) [![Test Status](https://img.shields.io/github/workflow/status/pascaliske/helm-charts/Test%20Charts/master?label=test&style=flat-square)](https://github.com/pascaliske/helm-charts/actions/workflows/test.yml) [![Build Status](https://img.shields.io/github/workflow/status/pascaliske/helm-charts/Release%20Charts/master?label=build&style=flat-square)](https://github.com/pascaliske/helm-charts/actions/workflows/release.yml) ![GitHub Last Release](https://img.shields.io/github/release-date/pascaliske/helm-charts?label=last%20release&style=flat-square) [![GitHub Last Commit](https://img.shields.io/github/last-commit/pascaliske/helm-charts?style=flat-square)](https://github.com/pascaliske/helm-charts) [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](https://opensource.org/licenses/MIT) [![Awesome Badges](https://img.shields.io/badge/badges-awesome-green.svg?color=blue&style=flat-square)](https://github.com/Naereen/badges)

## Usage

[Helm](https://helm.sh) must be installed to use the charts. Please refer to Helm's [documentation](https://helm.sh/docs) to get started. Once Helm has been set up correctly, add the repo as follows:

```sh
helm repo add pascaliske https://charts.pascaliske.dev
```

If you had already added this repo earlier, run `helm repo update` to retrieve the latest versions of the packages. Use `helm search repo pascaliske` to see a list of all available charts.

You can install a chart release using the following command:

```sh
helm install <release> pascaliske/<chart> --values values.yaml
```

To uninstall a chart release use `helm`'s delete command:

```sh
helm delete <chart>
```

## Charts

| Chart                                                                                                     | Version |     AppVersion     |
| --------------------------------------------------------------------------------------------------------- | :-----: | :----------------: |
| [`cloudflared`](https://github.com/pascaliske/helm-charts/tree/master/charts/cloudflared)                 | `1.1.0` |     `2022.1.0`     |
| [`code-server`](https://github.com/pascaliske/helm-charts/tree/master/charts/code-server)                 | `0.1.1` |      `v4.0.2`      |
| [`digitalocean-dyndns`](https://github.com/pascaliske/helm-charts/tree/master/charts/digitalocean-dyndns) | `0.2.0` |      `0.0.1`       |
| [`fritzbox-exporter`](https://github.com/pascaliske/helm-charts/tree/master/charts/fritzbox-exporter)     | `1.0.1` |       `1.0`        |
| [`gitlab`](https://github.com/pascaliske/helm-charts/tree/master/charts/gitlab)                           | `0.2.4` |   `14.7.2-ce.0`    |
| [`linkding`](https://github.com/pascaliske/helm-charts/tree/master/charts/linkding)                       | `0.0.1` |      `1.8.4`       |
| [`paperless`](https://github.com/pascaliske/helm-charts/tree/master/charts/paperless)                     | `0.0.2` |      `1.5.0`       |
| [`prometheus`](https://github.com/pascaliske/helm-charts/tree/master/charts/prometheus)                   | `1.2.0` |     `v2.33.1`      |
| [`redis`](https://github.com/pascaliske/helm-charts/tree/master/charts/redis)                             | `0.0.2` |      `6.2.6`       |
| [`snapdrop`](https://github.com/pascaliske/helm-charts/tree/master/charts/snapdrop)                       | `0.0.1` | `version-78a8b167` |
| [`traefik-errors`](https://github.com/pascaliske/helm-charts/tree/master/charts/traefik-errors)           | `1.0.2` |      `1.0.1`       |
| [`uptime-kuma`](https://github.com/pascaliske/helm-charts/tree/master/charts/uptime-kuma)                 | `0.0.5` |      `1.10.2`      |

## License

[MIT](LICENSE.md) ??? ?? 2022 [Pascal Iske](https://pascaliske.dev)
