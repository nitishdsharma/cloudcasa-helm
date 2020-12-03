# Cloudcasa
Cloudcasa is one of the most versatile SaaS solution to manage backups for your Kubernetes/Docker containers and Volumes.

## Introduction

This chart bootstraps a kube-agent deployment on a client Kuberntes [Kubernetes](http://kubernetes.io) cluster using the [Helm](https://helm.sh) package manager.

## Helm Chart installation modes

- CLI based installation
##### &nbsp;&nbsp;&nbsp;&nbsp; Update the value of AMDS_CLUSTER_ID and AMDS_CLUSTER_TYPE in the values.yaml file.

```
helm repo add cloudcasa https://nitishdsharma.github.io/cloudcasa-helm
helm search repo cloudcasa
helm install <release name> cloudcasa/cloudcasa-app -f values.yaml
```
- Helmchart hosted on Rancher Apps
```
- Register the cloudcasa helm chart repo in the Rancher Apps Repository.
- Go to charts select the repo -> Cloudcasa-app chart.
- Provide the name of release. 
- In cloudcasa setting section, provide the AMDS_CLUSTER_ID and the AMDS_CLUSTER_TYPE. 
- Click on Install button.
```

## Upgrade Notes
Can upgrade the existing/deployed helm release with the new helm chart version.
