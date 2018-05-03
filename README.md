# kubernetes-ingress-nginx

Ingress-nginx前提准备资源部署
    
    $ kubectl create -f namespace.yaml
    $ kubectl create -f default-backend.yaml
    $ kubectl create -f tcp-services-configmap.yaml 
    $ kubectl create -f udp-services-configmap.yaml

安装在有RBAC角色环境中

    $ kubectl create -f rbac.yaml 
    $ kubectl create -f with-rbac.yaml

安装在没有RBAC角色环境中

    $ kubectl create -f without-rbac.yaml


检查Pods资源运行情况

    $ kubectl get all -n ingress-nginx
    $ kubectl get pods -n ingress-nginx
    $ kubectl describe pods -n ingress-nginx

查看集群IP和端口
    
    $ kubectl get svc -n ingress-nginx


https://github.com/kubernetes/ingress-nginx/blob/master/docs/deploy/index.md
