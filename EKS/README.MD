# To create EKS on AWS we require some application:
## This cmd will work in ubuntu
- zip
- awscli
- kubectl
- eksctl

## Update and Upgrade the linux:
```bash
sudo apt-get update 
sudo apt-get upgrade -y
```

## First check the type:
```bash
uname -i
```

## zip install:
```bash
sudo apt-get install zip -y
```

## awscli installtion:
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

## kubectl install:
- got to site (https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/) and download the latest one
```bash
curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
```
```bash

```
