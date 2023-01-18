# Useful notes  

## Useful links  

[Spring Boot with Docker](https://spring.io/guides/gs/spring-boot-docker/)  
[Install Rancher Desktop on Linux](https://docs.rancherdesktop.io/getting-started/installation/#linux)  
[Manage Docker as a non-root user](https://docs.docker.com/engine/install/linux-postinstall/#manage-docker-as-a-non-root-user)  
[Minikube Installation](https://minikube.sigs.k8s.io/docs/start/)  
[Kubernetes Crash Course for Absolute Beginners](https://www.youtube.com/watch?v=s_o8dwzRlu4&t=2450s) [(Git Repo)](https://gitlab.com/nanuchi/k8s-in-1-hour)  
[Introduction to Helm | Kubernetes Tutorial | Beginners Guide](https://www.youtube.com/watch?v=5_J7RWLLVeQ&list=PLGemgmMsjljTRDg6KH4MPjw0hHY9MofPo&index=87) [(Git Repo)](https://github.com/marcel-dempers/docker-development-youtube-series/tree/master/kubernetes/helm)  
[How to Use Environment Variables with Helm Charts](https://phoenixnap.com/kb/helm-environment-variables)  

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

<code>docker build -t brunosantanati/gs-spring-boot-docker .</code>  
<code>docker run -p 8080:8080 brunosantanati/gs-spring-boot-docker</code>  
<code>docker login</code>  
<code>docker push brunosantanati/gs-spring-boot-docker</code>  

## Minikube commands  

<code>curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64</code>  
<code>sudo install minikube-linux-amd64 /usr/local/bin/minikube</code>  
<code>sudo snap install kubectl --classic</code>  
<code>minikube start --driver docker</code>  
<code>minikube status</code>  
<code>minikube stop --all</code>  
<code>minikube logs --file=logs.txt</code>  
<code>kubectl get node</code>  
<code>kubectl get node -o wide</code>  
<code>kubectl get service -o wide</code>  
<code>kubectl get deploy -o wide</code>  
<code>kubectl get pod</code>  
<code>kubectl get pod -o wide</code>  
<code>kubectl logs \<pod-name\></code>  
<code>kubectl logs \<pod-name\> -f</code>  
<code>kubectl exec \<pod-name\> -- printenv</code>  
<code>kubectl get svc</code>  
<code>kubectl get svc -o wide</code>  
<code>kubectl get cm</code>  
<code>kubectl get secret</code>  
<code>kubectl get all</code>  
<code>minikube ip</code>  
<code>kubectl apply -f webapp.yaml</code>  
<code>kubectl delete pod \<pod-name\></code>  
<code>kubectl delete svc \<service-name\></code>  
<code>kubectl delete deploy \<deployment-name\></code>  

Access the application deployed in the Kubernetes cluster:  
http://\<minikube-ip\>:\<node-port\>/  

## Helm commands  

Install Helm CLI  
```
curl -LO https://get.helm.sh/helm-v3.4.0-linux-amd64.tar.gz
tar -C /tmp/ -zxvf helm-v3.4.0-linux-amd64.tar.gz
rm helm-v3.4.0-linux-amd64.tar.gz
mv /tmp/linux-amd64/helm /usr/local/bin/helm
chmod +x /usr/local/bin/helm
```  

<code>helm create example-app</code>  
<code>helm template example-app example-app</code>  
<code>helm template example-app example-app --values ./example-app/values.yaml</code>  
<code>helm install example-app example-app</code>  
<code>helm install example-app example-app --values ./example-app/values.yaml</code>  
<code>helm list</code>  
<code>helm upgrade example-app example-app --values ./example-app/values.yaml</code>  
<code>helm delete example-app</code>  