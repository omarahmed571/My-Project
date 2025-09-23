# My-Project

Implemented GitOps based CI/CD pipeline using GitLab CI, Argo CD and Helm on Kubernetes.

# Architecture

<img width="1094" height="452" alt="My-Project" src="https://github.com/user-attachments/assets/72477e16-01ff-4d10-999e-f3d22f70fe6e" />

# Steps

-	Containerized a sample application with Docker and pushed images to a container registry.
-	Automated image build, tag and publish using GitLab CI pipeline.
-	Packaged Kubernetes manifests into Helm charts for templated deployments. 
-	Configured Argo CD to synchronize manifests from Git to Kubernetes for automated delivery.

# Tech-Stack

- GitLab CI → Continuous Integration & automation  
- Docker → Application containerization
- Kubernetes → Container orchestration platform
- Helm → Packaging Kubernetes manifests  
- Argo CD → GitOps-based Continuous Delivery

## Key-Features

** End to end automation from code commit to cluster deployment using: **
- Continous Integration via GitLab CI pipelines automating build and push of Docker images.  
- Helm Charts for templated Kubernetes manifests.  
- GitOps Workflow for declarative, version-controlled deployments.  
- Continuous Delivery via Argo CD syncing Git with Kubernetes.  
