# Cloudcasa
Cloudcasa is one of the most versatile SaaS solution to manage backups for your Kubernetes/Docker containers and Volumes.

## Introduction

This chart bootstraps a kube-agent deployment on a client Kuberntes [Kubernetes](http://kubernetes.io) cluster using the [Helm](https://helm.sh) package manager. This chart registers a client Kubernetes cluster to the Cloudcasa server.

## Installation
##### Update the value of AMDS_CLUSTER_ID in the values.yaml file.

```
1. helm repo add cloudcasa-repo https://catalogicsoftware.github.io/cloudcasa-helmchart
2. helm install <Chart Object Name> cloudcasa-repo/cloudcasa-helmchart --set AMDS_CLUSTER_ID=<CLUSTER ID VALUE>
```

### Upgrade steps
=================
- helm list -> This commands helps to list the already available helm objects or releases. Cloudcasa-helmchart Chart object should be listed.
- helm upgrade <Chart Object Name> cloudcasa-repo/cloudcasa-helmchart --set AMDS_CLUSTER_ID=<CLUSTER ID VALUE>
