# helm-charts-poc

https://helm.sh/docs/howto/chart_releaser_action/
https://github.com/helm/chart-releaser

## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

  helm repo add helm-charts-poc https://radoscis-org.github.io/helm-charts-poc

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
<alias>` to see the charts.

To install the <chart-name> chart:

    helm install my-<chart-name> <alias>/<chart-name>

To uninstall the chart:

    helm delete my-<chart-name>

## TO DO 
integrate with https://github.com/marketplace/actions/helm-chart-testing
and even https://github.com/marketplace/actions/kind-cluster