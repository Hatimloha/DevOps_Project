# To create EKS on AWS we require some application:
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

