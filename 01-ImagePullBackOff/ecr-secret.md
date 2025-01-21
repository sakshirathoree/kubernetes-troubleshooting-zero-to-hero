```

kubectl create secret docker-registry ecr-secret \
    --docker-server=<aws_account_id>.dkr.ecr.<region>.amazonaws.com \
    --docker-username=AWS \
    --docker-password=$(aws ecr get-login-password --region <region>) \
    --docker-email=<your_email@example.com>


```
