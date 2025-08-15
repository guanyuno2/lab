Cons of Docker:

1 applicattion have many replicate in another VM, it’s still scalable but hard to maintaince

======

kubectl create deploy test —image=http —replicas=3 (create a deployment)

kubectl run tyvan --image=nginx --dry-run=client -o yaml (create a pod with default yaml)

kubectl create deploy ty-deploy --image=http --replicas=10 --dry-run=client -o yaml > deploy.yaml

kubectl delete deployments.apps ty-deploy

Create a deployment first with number of replicas ⇒ it’ll create n replicas set with pod

Deployment  →  ReplicaSet  →  Pod

deployment by default have rollingUpdate 

deployment is apps/v1 controller to manage res 

Deployement manage ReplicaSet. ReplicaSet Manage Pod