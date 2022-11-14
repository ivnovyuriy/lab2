# itran-lab2

2.1 Installing minicube (microk8s on Apple silicon)

-> brew install ubuntu/microk8s/microk8s

![microk8s](https://github.com/ivnovyuriy/lab2/blob/master/img/1.png)

![microk8s](https://github.com/ivnovyuriy/lab2/blob/master/img/2.png)

![microk8s](https://github.com/ivnovyuriy/lab2/blob/master/img/3.png)

2.2 Create namespace

-> microk8s kubectl create namespace mynamespace

-> microk8s kubectl get namespaces

![namespace](https://github.com/ivnovyuriy/lab2/blob/master/img/5.png)

2.3 Deployment file to install nginx

-> microk8s kubectl apply -f main.yaml -n mynamespace

![deployment](https://github.com/ivnovyuriy/lab2/blob/master/img/6.png)

test deployment

-> microk8s kubectl get deployments --namespace=mynamespace

test pods

-> microk8s kubectl get pods --namespace=mynamespace

2.4 install ingress controller

-> microk8s enable ingress

![ingress](https://github.com/ivnovyuriy/lab2/blob/master/img/10.png)

2.5 Run commands

-> microk8s kubectl get pods -A

![pods](https://github.com/ivnovyuriy/lab2/blob/master/img/7.png)

-> microk8s kubectl get svc

![svc](https://github.com/ivnovyuriy/lab2/blob/master/img/8.png)

-> kubectl get all

![all](https://github.com/ivnovyuriy/lab2/blob/master/img/9.png)