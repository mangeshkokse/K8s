# 1 Explain Kubernetes Architecture

Kubernetes has a master-worker architecture, consisting of the following key components:

## 1. Master Node (Control Plane)
- **API Server**: Acts as the front-end, managing communication between components and users.
- **etcd**: A key-value store for all cluster data.
- **Scheduler**: Allocates pods to nodes based on resources and constraints.
- **Controller Manager**: Ensures the desired state of the cluster by managing various controllers (e.g., Node, Replication, Endpoint controllers).

## 2. Worker Nodes
- **Kubelet**: Manages the pod lifecycle and ensures containers are running.
- **Kube-proxy**: Handles networking and load balancing within the cluster.
- **Container Runtime**: Runs containers (e.g., Docker, containerd).

## 3. Pods
The smallest deployable unit, containing one or more containers.

---

Kubernetes uses this architecture to manage containerized applications across a distributed environment.
