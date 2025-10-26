# Docker Images

1. 建立 image: docker build -f XXX.dockerfile -t jadokao/XXX:1.0.0 .
2. 上傳 iamge 到 docker hub: docker push jadokao/XXX-service:1.0.0

# K8S cmd

1. 啟動 k8s server: kubectl apply -f k8s/broker.yml
2. minikube dashboard
3. minikube start --nodes=2
4. minikube status
5. kubectl get pods
6. kubectl logs broker-service-f49b956-tdfxz
7. kubectl get deployments
8. kubectl delete deployments broker-service mongo rabbitmq
9. kubectl get svc
10. kubectl delete svc broker-service mongo rabbitmq

# Docker Swarm

1. docker swarm init
2. docker swarm join-token worker
3. docker swarm join-token manager
4. docker stack deploy -c swarm.yml myapp
5. docker service ls
6. docker swarm leave --force
