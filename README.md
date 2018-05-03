# kubernetes-ingress-nginx

Ingress-nginx前提准备资源部署

    $ kubectl apply -f namespace.yaml
    $ kubectl apply -f default-backend.yaml
    $ kubectl apply -f tcp-services-configmap.yaml 
    $ kubectl apply -f udp-services-configmap.yaml

安装在有RBAC角色环境中

    $ kubectl apply -f rbac.yaml 
    $ kubectl apply -f with-rbac.yaml

安装在没有RBAC角色环境中

    $ kubectl apply -f without-rbac.yaml
