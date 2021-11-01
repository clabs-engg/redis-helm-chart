# [`gitlab`](https://github.com/pascaliske/helm-charts/tree/master/charts/gitlab)

> A Helm chart for GitLab Omnibus

[![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ](https://github.com/pascaliske/helm-charts/tree/master/charts/gitlab)[![Version: 0.0.2](https://img.shields.io/badge/Version-0.0.2-informational?style=flat-square) ](https://github.com/pascaliske/helm-charts/tree/master/charts/gitlab)[![AppVersion: 14.4.1-ce.0](https://img.shields.io/badge/AppVersion-14.4.1--ce.0-informational?style=flat-square) ](https://github.com/pascaliske/helm-charts/tree/master/charts/gitlab)

* <https://github.com/pascaliske/helm-charts>
* <https://docs.gitlab.com>

## Requirements

- [`helm`](https://helm.sh) - Refer to their [docs](https://helm.sh/docs) to get started.

## Usage

To use this chart add the repo as follows:

```sh
helm repo add pascaliske https://charts.pascaliske.dev
```

If you had already added this repo earlier, run `helm repo update` to retrieve the latest versions of the packages.

To install this chart simply run the following command:

```sh
helm install gitlab pascaliske/gitlab
```

To uninstall this chart simply run the following command:

```sh
helm delete gitlab
```

## Values

The following values can be used to adjust the helm chart.

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| backups.enabled | bool | `true` |  |
| backups.hostPath | string | `""` |  |
| backups.mountPath | string | `"/backups"` |  |
| configMap.annotations | object | `{}` |  |
| configMap.config | string | `"# external_url 'https://gitlab.example.com'\n"` |  |
| configMap.create | bool | `true` |  |
| configMap.existingConfigMap | string | `""` |  |
| configMap.labels | object | `{}` |  |
| configMap.mountPath | string | `"/etc/gitlab"` |  |
| deployment.annotations | object | `{}` |  |
| deployment.enabled | bool | `true` |  |
| deployment.kind | string | `"Deployment"` |  |
| deployment.labels | object | `{}` |  |
| deployment.replicas | int | `1` |  |
| env[0].name | string | `"TZ"` |  |
| env[0].value | string | `"UTC"` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"gitlab/gitlab-ce"` |  |
| image.tag | string | `"14.4.1-ce.0"` |  |
| nameOverride | string | `""` |  |
| persistentVolumeClaim.annotations | object | `{}` |  |
| persistentVolumeClaim.create | bool | `true` |  |
| persistentVolumeClaim.existingPersistentVolumeClaim | string | `""` |  |
| persistentVolumeClaim.labels | object | `{}` |  |
| persistentVolumeClaim.mountPath | string | `"/var/opt/gitlab"` |  |
| ports.http.enabled | bool | `true` |  |
| ports.http.nodePort | string | `nil` |  |
| ports.http.port | int | `80` |  |
| ports.http.protocol | string | `"TCP"` |  |
| resources | object | `{}` |  |
| securityContext | object | `{}` |  |
| service.annotations | object | `{}` |  |
| service.enabled | bool | `true` |  |
| service.labels | object | `{}` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.name | string | `""` |  |

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| pascaliske | info@pascaliske.dev | https://pascaliske.dev |

## License

[MIT](LICENSE.md) – © 2021 [Pascal Iske](https://pascaliske.dev)