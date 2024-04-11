# cluster-template-helm-charts
Contains demo Helm Charts for use with the
[cluster-templates-operator](https://github.com/stolostron/cluster-templates-operator/).
Refer to the Operator's documentation for more information.

To package a new chart run the following commands:

```shell
helm package <chart-dir>
helm repo index . --url https://amisstea.github.io/cluster-template-helm-charts
```