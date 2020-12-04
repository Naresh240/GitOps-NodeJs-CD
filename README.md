# Nodejs-helloworld

# Pre-requisites:
    - Install GIT
    - EKS Cluster
	- Install Docker
# EKS Cluster Setup:
  [EKS Cluster Setup](https://github.com/Naresh240/eks-cluster-setup/blob/main/README.md)
# Install GIT:
    yum install git -y
# Install Docker:
    yum install docker -y
    service docker start
# Clone code from github:
    git clone https://github.com/Naresh240/GitOps-NodeJs-CD.git
    cd GitOps-NodeJs-CD
# Build Docker image for Springboot Application
    docker build -t naresh240/nodejsdeploy:latest .
# Docker login
    docker login
# Push docker image to dockerhub
    docker push naresh240/nodejsdeploy:latest
