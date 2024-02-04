# Docker 설치 for Amazon Linux 2

## Docker 설치
```sh
    sudo yum update -y
    sudo yum install docker
    
    sudo usermod -aG docker $USER
    sudo newgrp docker
    sudo systemctl restart docker
```

## Docker-compose 설치

```sh
    sudo curl -L https://github.com/docker/compose/releases/latest/download/docker-compose-$(uname -s)-$(uname -m) -o /usr/local/bin/docker-compose

    sudo chmod +x /usr/local/bin/docker-compose
    
    ## symbolic 링크생성
    sudo ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose 
```

## 설치 확인

```sh
    ## docker 
    docker ps

    ## docker-compose
    docker-compose --version
```