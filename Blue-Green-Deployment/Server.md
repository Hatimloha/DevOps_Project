## Server

### Prerequisite
- Name: Server
- EC2: t2.micro
- install zip
- install awscli
- install terraform
- 

## Update the server 
```bash
sudo -i
apt-get update
apt-get upgrade -y
```

## Change the host name
```
vi etc/host
# remove everthing from the host file and type "Server"
```

## Restart the server
```bash
sudo init 6
```

## Check the System Type
```bash
uname -i
```

## 1. Install Zip:
```bash
sudo apt-get install zip -y
```

## 2. Install AWS CLI:
```bash
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
```

## Configure AWS CLI:
```bash
# Log in via IAM role (provide admin write access if you're a beginner)
aws configure
```
> You'll be prompted to enter the following:
- AWS Access Key ID [None]: Required
- AWS Secret Access Key [None]: Required
- Default region name [None]: Enter
- Default output format [None]: Enter

## 3. Install terraform
Ensure that your system is up to date and you have installed the gnupg, software-properties-common, and curl packages installed. You will use these packages to verify HashiCorp's GPG signature and install HashiCorp's Debian package repository.
```bash
sudo apt-get update && sudo apt-get install -y gnupg software-properties-common
```
- Install the HashiCorp GPG key.
```bash
wget -O- https://apt.releases.hashicorp.com/gpg | \
gpg --dearmor | \
sudo tee /usr/share/keyrings/hashicorp-archive-keyring.gpg > /dev/null
```
- Verify the key's fingerprint.
```bash
gpg --no-default-keyring \
--keyring /usr/share/keyrings/hashicorp-archive-keyring.gpg \
--fingerprint
```
Add the official HashiCorp repository to your system. The lsb_release -cs command finds the distribution release codename for your current system, such as buster, groovy, or sid.
```bash
echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] \
https://apt.releases.hashicorp.com $(lsb_release -cs) main" | \
sudo tee /etc/apt/sources.list.d/hashicorp.list
```
- Download the package information from HashiCorp.
```bash
sudo apt update
```
- Install Terraform from the new repository.
```bash
sudo apt-get install terraform
```
- Verify the installation
```bash
terraform -help
```
## 4. Clone the repo
```bash
git clone https://github.com/jaiswaladi246/Blue-Green-Deployment.git
```
- Go inside the git clone folder
```bash
cd Blue-Green-Deployment
```

- Go inside the Cluster folder
```bash
cd Cluster
```
## 5. Terraform
Initialize the Terraform
```bash
terraform init
```
- terraform plan is used to create an execution plan, showing what actions Terraform will take to reach the desired state defined in the configuration files.
```bash
terraform plan
```
- Before `terraform apply` check the region and zone in variables.tf file inside the Cluster folder
```bash

```
## 
```bash

```
## 
```bash

```
## 
```bash

```
## 
```bash

```
## 
```bash

```
## 
```bash

```
## 
```bash

```
## 
```bash

```
## 
```bash

```

