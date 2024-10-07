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
