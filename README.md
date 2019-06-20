# nodeapp-helm
## NOTE
If you get error like this
```
configmaps is forbidden: User "system:serviceaccount:kube-system:default" cannot list resource "configmaps" in API group "" in the namespace "kube-system"
```
### To deploy triller service account RBAC
```
kucbectl create -f https://raw.githubusercontent.com/javahometech/nodeapp-helm/master/rbac/rbac-config.yaml
```
### To intial helm local repository
```
helm init
```
### To create helm chart
```
helm create nodeapp-helm
```
### To create helm package
```
helm package nodeapp-helm
```
### To deploy helm package
```
helm install nodeapp-helm
```
### To list out helm deployments
```
helm ls
```
### To delete helm deployments
```
helm delete helm-deployment-name
```
