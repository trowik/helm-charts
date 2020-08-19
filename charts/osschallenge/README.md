osschallenge
============
Chart for osschallenge application

Current chart version is `0.1.0`


**Homepage:** <https://github.com/trowik/osschallenge>


## Maintainers
This chart is maintained by [Adfinis](https://adfinis.com/?pk_campaign=github&pk_kwd=helm-charts).


## Source Code

* <https://github.com/trowik/osschallenge>
* <https://github.com/trowik/helm-charts/tree/master/charts/osschallenge>


## Chart Requirements


| Repository | Name | Version |
|------------|------|---------|
| https://charts.bitnami.com/bitnami | postgresql | `~9.1.1` |
## Chart Values


| Key | Type | Default | Description |
|-----|------|---------|-------------|
| `ingress.annotations` | object | `{}` | Ingress annotations |
| `ingress.enabled` | bool | `false` | Enable ingress for osschalenge |
| `ingress.hosts` | list | `["localhost"]` | Ingress hostnames |
| `ingress.tls` | list | `[]` | Ingress TLS options |
| `osschallenge.image.pullPolicy` | string | `"IfNotPresent"` |  |
| `osschallenge.image.repository` | string | `"adfinissygroup/oss-challenge"` |  |
| `osschallenge.image.tag` | string | `nil` |  |
| `osschallenge.livenessProbe.enabled` | bool | `true` |  |
| `osschallenge.livenessProbe.failureThreshold` | int | `6` |  |
| `osschallenge.livenessProbe.initialDelaySeconds` | int | `60` |  |
| `osschallenge.livenessProbe.periodSeconds` | int | `10` |  |
| `osschallenge.livenessProbe.successThreshold` | int | `1` |  |
| `osschallenge.livenessProbe.timeoutSeconds` | int | `5` |  |
| `osschallenge.readinessProbe.enabled` | bool | `true` |  |
| `osschallenge.readinessProbe.failureThreshold` | int | `6` |  |
| `osschallenge.readinessProbe.initialDelaySeconds` | int | `30` |  |
| `osschallenge.readinessProbe.periodSeconds` | int | `10` |  |
| `osschallenge.readinessProbe.successThreshold` | int | `1` |  |
| `osschallenge.readinessProbe.timeoutSeconds` | int | `5` |  |
| `osschallenge.replicaCount` | int | `1` |  |
| `osschallenge.resources` | object | `{}` |  |
| `osschallenge.service.externalPort` | int | `8000` |  |
| `osschallenge.service.internalPort` | int | `8000` |  |
| `osschallenge.service.name` | string | `"osschalenge"` |  |
| `osschallenge.service.type` | string | `"ClusterIP"` |  |
| `osschallenge.settings.emailFrom` | string | `"osschallenge@osschallenge.com"` |  |
| `osschallenge.settings.emailHost` | string | `"smtp.examplexample.ch:587"` |  |
| `osschallenge.settings.serverEmail` | string | `"osschallenge@osschallenge.com"` |  |
| `postgresql.enabled` | bool | `true` | Enable PostgreSQL for persistence |
| `postgresql.postgresqlDatabase` | string | `"osschallenge"` | PostgreSQL database name |
| `postgresql.postgresqlPassword` | string | `nil` | Set a password for PostgreSQL |
| `postgresql.postgresqlUsername` | string | `"postgres"` | PostgreSQL user name |

## About this chart

Adfinis fights for a software world that is more open, where the quality is
better and where software must be accessible to everyone. This chart
is part of the action behind this commitment. Feel free to
[contact](https://adfinis.com/kontakt/?pk_campaign=github&pk_kwd=helm-charts)
us if you have any questions.

## License

This Helm chart is free software: you can redistribute it and/or modify it under the terms
of the GNU Affero General Public License as published by the Free Software Foundation,
version 3 of the License.
