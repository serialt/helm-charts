# Helm Charts

## Serialt Helm Charts


## Usage

```shell
helm repo add serialt https://serialt.github.io/helm-charts
```

## Example

### update rpeo 
```shell
[serialt@Sugar ~]$ helm repo update serialt
Hang tight while we grab the latest from your chart repositories...
...Successfully got an update from the "serialt" chart repository
Update Complete. ⎈Happy Helming!⎈
```

### search repo
```shell
[root@serialt ~]# helm repo list
NAME    URL                                 
serialt https://serialt.github.io/helm-charts
```
You can then run helm search repo serialt to see the charts.

```
[root@serialt ~]# helm search repo
NAME            CHART VERSION   APP VERSION     DESCRIPTION                
serialt/test    0.1.0           1.16.0          A Helm chart for Kubernetes
```

### install chart

```shell
[root@serialt ~]# helm install nginx-demo serialt/test --version=0.1.0
```