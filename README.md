# promptfoo helm chart


### Introduction

This chart bootstraps a [promptfoo]() deployment on a [Kubernetes](http://kubernetes.io) cluster using the [Helm](https://helm.sh) package manager.

### Prerequisites
make sure you are connected to the correct cluster (uat-k8s) by running the following command:
```bash
kubectl get nodes
```

### Installing the Chart
to install the chart into `ops-uat` namespace, run the following command:
```bash
helm upgrade --install promptfoo-server . -nops-uat
```

### Uninstalling the Chart
```bash
### DO NOT DO THAT
# its documented here for reference only
# it will delete the PVC with all users evaluations data
helm uninstall promptfoo-server -nops-uat
```
