## Manage Deployments in Kubernetes

##### Update Container Image

To update the container image of a deployment:

`kubectl set image deploy nginx-deployment nginx=nginx:1.17.1 `

##### Deployment Rollout History
View the rollout history of a deployment:

`kubectl rollout history deployment/nginx-deployment`

View specific revision details:

`kubectl rollout history deployment/nginx-deployment --revision=2`

##### Scale Deployment
Scale the number of replicas in a deployment:

`kubectl scale deployment/nginx-deployment --replicas=10`

##### Autoscale Deployment
Autoscale a deployment based on CPU usage:

`kubectl autoscale deployment/nginx-deployment --min=10 --max=15 --cpu-percent=80`

##### Pause Deployment Rollout
Pause the rollout of a deployment:

`kubectl rollout pause deployment/nginx-deployment`

##### Modify Resource Limits

Set resource limits for containers in a deployment:

`kubectl set resources deployment/nginx-deployment -c=nginx --limits=cpu=200m,memory=512`