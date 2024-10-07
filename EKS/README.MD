# Nginx Server on AWS EKS
## Description
This repository contains configurations and scripts to deploy an Nginx server on AWS Elastic Kubernetes Service (EKS).

## Prerequisites
- AWS Account
- ec2 (t2.micro)
- zip
- awscli
- kubectl
- eksctl

## Setup Instructions
1. Clone this repository.
2. Install dependencies.
3. Configure AWS CLI.

## Update and Upgrade the linux:
```bash
sudo apt-get update 
sudo apt-get upgrade -y
```

## First check the type:
```bash
uname -i
```

## 1. zip install:
```bash
sudo apt-get install zip -y
```

## 2. awscli installtion:
```bash
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
```

## Login AWS via CLI
```bash
# Login via IAM role (Provide admin write if you are a beginar)
aws configure
```
```bash
AWS Access Key ID [None]: Required
AWS Secret Access Key [None]: Required
Default region name [None]: Enter
Default output format [None]: Enter
```

## 3. kubectl install:
- Download the latest release with the command available on official docs: (https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/)
```bash
curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
```
- Validate the binary (optional)
```bash
curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl.sha256"

# Validate the kubectl binary against the checksum file:
echo "$(cat kubectl.sha256)  kubectl" | sha256sum --check

# If valid, the output is: 
## kubectl: OK
```
- Install kubectl
```bash
sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl
```

### If you do not have root access on the target system, you can still install kubectl to the ~/.local/bin directory:
```bash
chmod +x kubectl
mkdir -p ~/.local/bin
mv ./kubectl ~/.local/bin/kubectl
# and then append (or prepend) ~/.local/bin to $PATH
```

### Test to ensure the version you installed is up-to-date
```bash
kubectl version --client
```

## 4. Install eksctl
```bash
curl --silent --location "https://github.com/weaveworks/eksctl/releases/latest/download/eksctl_Linux_amd64.tar.gz" | tar xz -C /tmp
sudo mv /tmp/eksctl /usr/local/bin
```
- Verify the installation:
```bash
eksctl version
```
- Create an EKS Cluster (it will take 15-30 minute)
```bash
# Change require: <your-region>
# Change require: cluster-name
eksctl create cluster --name my-cluster --region <your-region> --node-type t2.micro --nodes 2
```
- Configure kubectl to Use the New Cluster
```bash
kubectl get svc
```
- Clean Up (Optional)
```bash
# Change require: <your-region>
# Change require: cluster-name
eksctl delete cluster --name my-cluster --region <your-region>
```

## 5. Apply the manifest:
- nginx-deployment.yaml
- nginx-service.yaml
```bash
kubectl apply -f nginx-deployment.yaml
kubectl apply -f nginx-service.yaml
```
- 
```bash

```
