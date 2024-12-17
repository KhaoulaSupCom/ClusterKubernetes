# LAB10: Kubernetes

## Objectives
1. **Create a Kubernetes Cluster** using EC2 instances.
2. **Deploy an Nginx web server**.

## Steps Overview

### 1. Virtual Machine Setup
- Three EC2 instances with the following specifications:
  - **AMI**: Ubuntu 18.04.6 LTS
  - **Instance Type**: t2.medium (2 vCPU, 4GB RAM)
  - **Storage**: 8GB
- Create a security group named **"k8s-Security Group"** to allow all traffic.

### 2. Installation and Configuration
- Add Kubernetes repository to the package manager.
- Install necessary Kubernetes components: `kubeadm`, `kubectl`, `kubelet`.
- Disable swap and configure the Kubernetes network.

### 3. Master Node Initialization
- Initialize the control plane using `kubeadm`.
- Configure access to the cluster with `kubectl`.

### 4. Worker Node Setup
- Join worker nodes to the cluster using the `kubeadm join` command.

### 5. Deployment of Nginx
- Deploy an Nginx web server using the official deployment descriptor.
- Scale the number of Nginx pods as needed using `kubectl edit deploy`.

---

This completes the LAB10 Kubernetes setup and deployment.
