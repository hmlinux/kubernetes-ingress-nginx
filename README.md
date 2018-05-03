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

https://github.com/kubernetes/ingress-nginx/blob/master/docs/deploy/index.md
