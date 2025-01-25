## basic commands:

1.  kubectl create ns secure-ns
2.  kubectl apply -f db.yaml 
3.  kubectl get pods -n secure-ns
4.  kubectl describe pod <pod-id> -n secure-ns

#### 1.  access the pod's shell
```
kubectl exec -it <redis-pod> -n secure-ns -- /bin/bash
```

#### 2. Access the Redis CLI inside the pod: Once inside the pod, you can access the Redis CLI using the following command
```
redis-cli
```

**If Redis is secured with a password, you will need to use the -a flag to authenticate:**
```
redis-cli -a <your-redis-password>
```
