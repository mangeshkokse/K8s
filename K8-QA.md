
# 1 What is Kubernetes?

Kubernetes is an open-source platform for automating the deployment, scaling, and management of containerized applications. It helps in managing clusters of containers across multiple hosts, ensuring that your applications run efficiently and remain available.

## Key Advantages of Kubernetes:

1. **Automated Scaling**: Dynamically adjusts the number of running containers based on demand.
2. **Self-healing**: Automatically replaces failed containers, reschedules containers when nodes fail, and restarts containers when they go down.
3. **Load Balancing**: Distributes traffic across containers to ensure stability and efficiency.
4. **Resource Optimization**: Automatically manages resources, helping to optimize infrastructure costs.
5. **Declarative Configuration**: Allows for defining the desired state of applications and automatically maintains it.
6. **Cross-Cloud Compatibility**: Runs on various environments, including on-premise, cloud (AWS, GCP, Azure), and hybrid environments.

---

Kubernetes is a powerful tool for managing modern, distributed applications.

# 2 Explain Kubernetes Architecture

Kubernetes has a master-worker architecture, consisting of the following key components:

## 1. Master Node (Control Plane)
- **Kube API Server**: Acts as the front-end, managing communication between components and users.
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

# 3 How are Kubernetes and Docker Linked?

- **Docker** is a platform for building, packaging, and running containers. It helps developers create isolated environments for applications using container images.
- **Kubernetes** is an orchestration platform that automates the deployment, scaling, and management of these containers across multiple machines (nodes).

In essence, Docker creates and runs containers, while Kubernetes manages and coordinates them across clusters, ensuring high availability and scalability. Kubernetes can work with Docker as the container runtime, though it also supports other runtimes like containerd.

