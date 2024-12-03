# Mirantis Telemetry Regional Stack
- grafana
- victoria-metrics operator
- vmcluster
- vmauth

## Cluster requirements
- cert-manager
- ingress-nginx

## Deploy
```
helm install .. --set victoriametrics.vmauth.ingress.host=vmauth.hmc0.weystrom.net --set grafana.ingress.host=grafana.hmc0.weystrom.net
```
victoriametrics:
  vmauth:
    ingress:
      host: vmauth.hmc0.weystrom.net
grafana:
  ingress:
    host: grafana.hmc0.weystrom.net