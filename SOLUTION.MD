  # Kubernetes Challenge
Deploy an application to minikube by feteching local image

Steps Followed:
1. Installed minikube on Ubuntu 20.04
2. Installed ca-certificates, curl, gnupg, lsb-release package
3. Added Docker offical GPG key
4. Ran Yum Update to update the repository list
5. Installed Docker engine & Docker CLI
6. Added user "Ubuntu" to docker group using `sudo usermod -aG docker $USER`
7. Activated changes to the group without without using `newgrp docker`
8. Set docker default driver using `minikube config set driver docker` command.
9. Installed kubectl
10. Started minikube using `minikube start`
11. Ran `eval $(minikube -p minikube docker-env)`
12. Build docker image using `docker build -t sample-app .`
13. Created Deployment YAML configuration and deployed.
14. Created Service YAML config and used kubectl to create the service.
15. Output of `curl $(minikube ip):30080` 
Hello MINIKUBE! 

# Challenges & Pending
- Limited upskilling time, no prior knowledge
- Pending ingress & configmap
