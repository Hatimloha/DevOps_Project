## Prerequisites
- AWS Account
- ec2 (t2.medium)
- java (jdk17)
- 

## Updating and Upgrading the System
```bash
sudo apt-get update 
sudo apt-get upgrade -y
```

## Check the System Type
```bash
sudo uname -i
```



## 1. Java
```bash
sudo apt install openjdk-17-jre-headlesss
```

## 2. Jenkins
Weekly release
A new release is produced weekly to deliver bug fixes and features to users and plugin developers. It can be installed from the debian apt repository.
```bash
sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian/jenkins.io-2023.key
echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]" \
  https://pkg.jenkins.io/debian binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt-get update
sudo apt-get install jenkins
```
- Enable jenkins service:
When ever server restartt jenkins service will be auto start
```bash
sudo systemctl enable jenkins
```
- login to the jenkins server
Copy public ip and paste in browser with port 8080
```bash
sudo cat /var/jenkins_home/secrets/initialAdminPassword
```
- click Install suggested plugin 
