1. start minikube
2. kubectl apply --filename deployment.yaml,service.yaml
3. kubectl create configmap nginx-conf --from-file=./nginx.conf
4. kubectl port-forward service/nginx 8080:80

**after:**
kubectl delete --all deployments,pods,services,replicaset
