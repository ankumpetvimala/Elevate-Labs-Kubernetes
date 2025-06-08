# Task 5: Kubernetes Cluster with Minikube

This repository contains my solution for **Task 5** of the DevOps Internship: setting up a Kubernetes cluster using **Minikube** on an AWS **Ubuntu EC2** instance, deploying an **Nginx** application, and exposing it using a **NodePort** service accessible on the EC2 public IP.

---

## Overview

- **Kubernetes** set up via **Minikube** on an EC2 Ubuntu instance.
- Deployed an **Nginx** application with 2 replicas initially.
- Exposed using a **NodePort** on port **30007**, accessible via EC2 public IP.
- Scaled deployment to 4 replicas.
- Verified access and cluster state with `kubectl`.

---

## Files Included

| File            | Description                                      |
|-----------------|--------------------------------------------------|
| `deployment.yaml` | Kubernetes Deployment for Nginx (2 replicas)     |
| `service.yaml`    | NodePort Service exposing Nginx on port 30007   |
| `pods.txt`        | Output of `kubectl get pods`                    |
| `services.txt`    | Output of `kubectl get services`                |

---

## Steps Performed

1. Launched an Ubuntu EC2 instance.
   
2. Installed:
   - Docker
   - `kubectl`
   - `minikube`

 3. Started Minikube with Docker driver:
   
 4.Created and applied deployment.yaml for Nginx.

 5.Exposed the app with service.yaml (NodePort 30007).

 6.Scaled the deployment to 4 replicas.

 7.Verified pods, services, and accessed the app at http://<ec2-public-ip>:30007.

## Access

The Nginx app is accessible at http://<ec2-public-ip>:30007 (replace with actual IP).

## Notes

Ensure EC2 security group allows port 30007.

Screenshots of the browser and terminal outputs are included or linked.
