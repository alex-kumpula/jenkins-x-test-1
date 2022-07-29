# jx3-kubernetes

Jenkins X 3.x GitOps repository for a vanilla Kubernetes cluster
        
[![Jenkins X Releases](https://img.shields.io/badge/Jenkins%20X-Releases-blue)](docs/README.md)



Two ports are exposed to your machine via K3D:

Port 80 -> 8085 (HTTP)
Port 443 -> 8086 (HTTPS)

This means you must port-forward port 8080 -> 80 and port 8081 -> 443 in your networking environment for this cluster to be accessible outside of your local network.


# 1. Start the cluster with K3D
k3d cluster create --config k3d-config.yaml