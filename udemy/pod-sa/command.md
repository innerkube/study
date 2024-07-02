
# serviceaccount command

```
kubectl get serviceaccount

kubectl get pods/<podname> -o yaml

kubectl get serviceaccounts/build-robot -o yaml

kubectl create token build-robot

kubectl create -f https://k8s.io/examples/pods/pod-projected-svc-token.yaml
```


## Set deployment nginx-deployment's service account to serviceaccount1

> kubectl set serviceaccount deployment nginx-deployment serviceaccount1

# Print the result (in YAML format) of updated nginx deployment with the service account from local file, without hitting the API server

> kubectl set sa -f nginx-deployment.yaml serviceaccount1 --local --dry-run=client -o yaml
