# My-Project

Implemented GitOps based CI/CD pipeline using GitLab CI, Argo CD and Helm on Kubernetes.

# Architecture

<img width="1094" height="452" alt="My-Project" src="https://github.com/user-attachments/assets/72477e16-01ff-4d10-999e-f3d22f70fe6e" />

# Workflow

-	Containerized a sample application with Docker and pushed images to container registry.
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

## Detailed-Steps

- Created 2 gitlab repos: code-repo and manifest-repo
1) code-repo: contains application source code + `.gitlab-ci.yml`
2) manifest-repo: contains Kubernetes manifests and Helm charts for deployment
- Cloned the repos to local machine to add source codes and manifests then push again to GitLab
- Created .gitlab-ci.yml file on code-repo to build image, push to container registry and update Helm Chart for deployment
- Connected Argo CD with my GitLab account through username and PAT(personal access token) and added manifest repo to Argo CD
- Created new app on Argo CD by defining source repo, path, targeted cluster and sync policy

## Results

<img width="1014" height="475" alt="image" src="https://github.com/user-attachments/assets/240deae5-9d21-4d3b-ae53-74dd17d5c761" />


<img width="1913" height="711" alt="image" src="https://github.com/user-attachments/assets/f99bedcc-e6ea-4761-96b8-2c6d657a2aac" />






