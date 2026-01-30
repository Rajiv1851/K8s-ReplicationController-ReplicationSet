# Kubernetes Learning – ReplicationController & ReplicaSet

Date: 30 January 2026

## Topics Covered
- ReplicationController
- ReplicaSet
- Scaling replicas from terminal
- Labels and selectors
- Watching Kubernetes resources

## ReplicationController (RC)

Create ReplicationController:
kubectl apply -f rc.yml

Check ReplicationController:
kubectl get rc

Describe ReplicationController:
kubectl describe rc myrc

## ReplicaSet (RS)

Create ReplicaSet:
kubectl apply -f rs.yml

Check ReplicaSet:
kubectl get rs

## Scaling Replicas from Terminal

Scale ReplicationController:
kubectl scale rc myrc --replicas=5

Scale ReplicaSet:
kubectl scale rs myrs --replicas=4

Verify Pods:
kubectl get pods

## Labels & Selectors

Show labels on pods:
kubectl get pods --show-labels

Filter pods using labels:
kubectl get pods -l app=myapp

## Watch Resources in Real-Time

Watch pods:
kubectl get pods -w

Watch ReplicaSet:
kubectl get rs -w

## Key Learnings
- ReplicationController maintains desired pod count
- ReplicaSet is modern replacement for RC
- Scaling without editing YAML
- Labels help group and manage resources
- Watch helps in real-time monitoring

## Author
Rajiv Nakhawa  
Cloud & DevOps Learner | Kubernetes | Docker | AWS

