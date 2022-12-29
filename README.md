# Useful notes  

## Useful links  

[Spring Boot with Docker](https://spring.io/guides/gs/spring-boot-docker/)  
[Install Rancher Desktop on Linux](https://docs.rancherdesktop.io/getting-started/installation/#linux)  
[Manage Docker as a non-root user](https://docs.docker.com/engine/install/linux-postinstall/#manage-docker-as-a-non-root-user)  
[Minikube Installation](https://minikube.sigs.k8s.io/docs/start/)  
[Kubernetes Crash Course for Absolute Beginners](https://www.youtube.com/watch?v=s_o8dwzRlu4&t=2450s)  

## Docker commands  

<code>sudo snap install docker</code>  
<code>sudo groupadd docker</code>  
<code>sudo usermod -aG docker $USER</code>  
<code>newgrp docker</code>  
<code>docker build -t springio/gs-spring-boot-docker .</code>  
<code>docker run -p 8080:8080 springio/gs-spring-boot-docker</code>  
<code>docker ps --all</code>  
<code>docker rm \<container-name\></code>  
<code>docker image ls --all</code>  
<code>docker rmi \<image-id\></code>  

## Minikube commands  

<code>curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64</code>  
<code>sudo install minikube-linux-amd64 /usr/local/bin/minikube</code>  
<code>sudo snap install kubectl --classic</code>  
<code>minikube start --driver docker</code>  
<code>minikube status</code>  
<code>kubectl get node</code>  
