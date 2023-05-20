# Helm Charts

## Serialt Helm Charts


## Usage

```shell
helm repo add serialt https://serialt.github.io/helm-charts
```

## Example

### search repo
```shell
[root@serialt ~]# helm repo list
NAME    URL                                 
serialt https://serialt.github.io/helm-charts
```
You can then run helm search repo grafana to see the charts.

```
[root@serialt ~]# helm search repo
NAME            CHART VERSION   APP VERSION     DESCRIPTION                
serialt/test    0.1.0           1.16.0          A Helm chart for Kubernetes
```

### install chart

```shell
[root@serialt ~]# helm install cc serialt/test
```