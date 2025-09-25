# My-Project

Implemented GitOps based CI/CD pipeline using GitLab CI, Argo CD and Helm on Kubernetes.

Check GitLab Repos: https://gitlab.com/Omar.Ahmed.7401/code-repo & https://gitlab.com/Omar.Ahmed.7401/manifest-repo

# Architecture

<img width="1094" height="452" alt="My-Project" src="https://github.com/user-attachments/assets/72477e16-01ff-4d10-999e-f3d22f70fe6e" />

# Workflow

-	Containerized a sample application with Docker and pushed images to container registry.
-	Automated image build, tag and publish using GitLab CI pipeline.
-	Packaged Kubernetes manifests into Helm charts for templated deployments. 
-	Configured Argo CD to synchronize manifests from Git to Kubernetes for automated deployments.

# Tech-Stack

- GitLab CI → Continuous Integration & automation  
- Docker → Application containerization
- Kubernetes → Container orchestration platform
- Helm → Packaging Kubernetes manifests  
- Argo CD → GitOps-based Continuous Deployment

# Key-Features

** End to end automation from code commit to cluster deployment using: **
- Continous Integration via GitLab CI pipelines automating build and push of Docker images.  
- Helm Charts for templated Kubernetes manifests.  
- GitOps Workflow for declarative, version-controlled deployments.  
- Continuous Deployment via Argo CD syncing Git with Kubernetes.

# Detailed-Steps

- Created 2 gitlab repos: code-repo and manifest-repo
1) code-repo: contains application source code + `.gitlab-ci.yml` Check it here: https://gitlab.com/Omar.Ahmed.7401/code-repo
2) manifest-repo: contains Kubernetes manifests and Helm charts Check it here: https://gitlab.com/Omar.Ahmed.7401/manifest-repo
- Cloned the repos to local machine to add source codes and manifests then push again to GitLab
- Created .gitlab-ci.yml file on code-repo to build image, push to container registry and update Helm Chart for deployments
- Connected Argo CD with my GitLab account through username and PAT(personal access token) and added manifest repo to Argo CD
- Created new app on Argo CD by defining source repo, path, targeted cluster and sync policy

# Results

GitLab CI pipeline ran successfully:

<img width="1014" height="475" alt="image" src="https://github.com/user-attachments/assets/240deae5-9d21-4d3b-ae53-74dd17d5c761" />

Argo CD synced manifests successfully:

<img width="1913" height="711" alt="image" src="https://github.com/user-attachments/assets/f99bedcc-e6ea-4761-96b8-2c6d657a2aac" />

Application deployed to Kubernetes cluster successfully:

<img width="1214" height="375" alt="image" src="https://github.com/user-attachments/assets/921ea162-5129-4cbf-a80a-9655e27bc951" />

Proof:

<img width="1915" height="846" alt="image" src="https://github.com/user-attachments/assets/373cfc42-73ad-4785-8906-47a99e44224c" />





