# Useful notes  

## Useful links  

[Spring Boot with Docker](https://spring.io/guides/gs/spring-boot-docker/)  
[Install Rancher Desktop on Linux](https://docs.rancherdesktop.io/getting-started/installation/#linux)
[Manage Docker as a non-root user](https://docs.docker.com/engine/install/linux-postinstall/#manage-docker-as-a-non-root-user)
[Minikube Installation](https://minikube.sigs.k8s.io/docs/start/)

## Docker commands  

<code>sudo snap install docker</code>  
<code>docker build -t springio/gs-spring-boot-docker .</code>  
<code>docker run -p 8080:8080 springio/gs-spring-boot-docker</code>  
<code>docker ps --all</code>  
<code>docker rm <container-name></code>  
<code>docker image ls --all</code>  
<code>docker rmi <image-id></code>  

## Minikube commands  

<code>curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64</code>  
<code>sudo install minikube-linux-amd64 /usr/local/bin/minikube</code>  
<code>minikube start --driver docker</code>  
<code>minikube status</code>  
