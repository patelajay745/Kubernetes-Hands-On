## Taint and toleration

`k taint nodes gke-cluster-2-default-pool-e5f12872-906g key1=value1:NoSchedule`

## To remove

`k taint nodes gke-cluster-2-default-pool-e5f12872-906g key1=value1:NoSchedule-`

## To see all tainted nodes

`kubectl get nodes -o custom-columns=NAME:.metadata.name,TAINTS:.spec.taints --no-headers`
