# charts

# Add repo before using
$ helm repo add ndtiendut https://raw.githubusercontent.com/ndtiendut/charts/master/
```
# Search for charts, or list all the charts by repo's name
$ helm search repo name
NAME                    CHART VERSION   APP VERSION     DESCRIPTION
ndtiendut/mynginx       0.1.0           1.16.0          A Helm chart for Kubernetes
ndtiendut/nginx2        0.1.0           1.16.0          A Helm chart for Kubernetes
```
# Get configurations (values file)
$ helm show values ndtiendut/mynginx > myvalues.yaml

# Install chart with your configurations
$ helm install mynginxtest ndtiendut/mynginx -f myvalues.yaml
```
