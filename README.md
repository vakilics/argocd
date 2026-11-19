# argocd-lab

Argocd-lab for teseting... 

* Portforwardning if required:

```
kubectl port-forward svc/argocd-server -n argocd 8080:443

kubectl port-forward svc/biotronik-welcome 8081:80

#Pass
kubectl get secret argocd-initial-admin-secret \         
-n argocd \
-o jsonpath="{.data.password}" | base64 -d
```
