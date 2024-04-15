# cluster-template-helm-charts
Contains demo Helm Charts for use with the
[cluster-templates-operator](https://github.com/stolostron/cluster-templates-operator/).
Refer to the Operator's documentation for more information.

To install a chart/create a cluster (and infra/iam):

```shell
helm install --wait --wait-for-jobs --timeout 20m my-cluster <chart-dir>
```

To uninstall a chart/destroy a cluster (and infra/iam):

```shell
helm uninstall --timeout 20m my-cluster
```

To package a new chart run the following commands:

```shell
helm package <chart-dir>
helm repo index . --url https://amisstea.github.io/cluster-template-helm-charts
```