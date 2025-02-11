# Cluster API Helm Chart
A Helm chart to install Cluster API manifests 

* Installs the [cluster API Manifests](cluster-api.sigs.k8s.io).

*Note: Currently the chart install a targer cluster in AWS. However it is intended to incude the support for other Cluster API providers.*

## Resources
https://medium.com/condenastengineering/clusterapi-a-guide-on-how-to-get-started-ff9a81262945
https://medium.com/swlh/clusterops-manage-your-kubernetes-clusters-with-gitops-ac5622f11ac6
https://medium.com/swlh/clusterops-1-line-commit-to-upgrade-your-kubernetes-clusters-de3548124d04

## Installing the Chart using ArgoCD

More details: https://github.com/kgamanji/cluster-api-argocd

To install the chart using ArgoCD use the following command:
```
kubectl apply -f argocd/application-capi.yaml
```

## Installing the Chart

To install the chart with the release name `my-release`:

***TO BE IMEPMELENTED*** 
```bash
## helm install kgamanji/cluster-api-aws
```


## Configuration

| Parameter                                    | Description                                                                           | Default                                    |
|:---------------------------------------------|:--------------------------------------------------------------------------------------|:-------------------------------------------|
| `kube.version`                           | Kubernetes version to be installed on the target clusters                                 | `v1.18.8`        |
| `master.replicas`                                  | Amount of master nodes in the target cluster                                                     | `3`                                   |
| `workers.replica`                           | Amount of worker nodes in the target cluster                                                                    | `3`                             |
