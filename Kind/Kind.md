# Installing Kubernetes using kind on Ubuntu

## Prerequisites

1. **Docker**: Ensure Docker is installed and running. If you don’t have Docker, install it with the following commands:

   ```bash
   sudo apt update
   sudo apt install -y apt-transport-https ca-certificates curl software-properties-common
   curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
   sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
   sudo apt update
   sudo apt install -y docker-ce
    ```
### After installation, ensure Docker is running:
