# Docker
commands used to create containers on docker
<hr>
**Commands:**
- curl -sL https://github.com/ShubhamTatvamasi/docker-install/raw/master/docker-install.sh | bash
- sudo apt update
sudo apt install -y \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg \
    lsb-release \
    jq
  - curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
  - echo \
  "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
- sudo apt update
sudo apt install -y docker-ce docker-ce-cli containerd.io
- sudo usermod -aG docker $USER
- COMPOSE_VERSION=$(curl -s "https://api.github.com/repos/docker/compose/tags" | jq -r '.[0].name')
sudo curl -L "https://github.com/docker/compose/releases/download/${COMPOSE_VERSION}/docker-compose-$(uname -s)-$(uname -m)" \ o /usr/local/bin/docker-compose
  - sudo chmod +x /usr/local/bin/docker-compose
  - docker pull hello-world
  - docker pull nginx
  - docker run -d -p 80:80 --name httpd-nginx httpd
  - docker stop nginx
  - docker rm nginx
  - docker pull httpd
  - docker run -d -p 80:80 --name httpd-apache httpd
