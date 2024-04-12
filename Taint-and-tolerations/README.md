## Taint and toleration


`k taint nodes gke-cluster-2-default-pool-e5f12872-906g key1=value1:NoSchedule`

## To remove

`k taint nodes gke-cluster-2-default-pool-e5f12872-906g key1=value1:NoSchedule-`


## To see all tainted nodes

`kubectl get nodes -o custom-columns=NAME:.metadata.name,TAINTS:.spec.taints --no-headers`

This repository is my trusty logbook, documenting every twist and turn of my Kubernetes adventure. Expect to find:

Daily Hands-on Labs: Buckle up for practical exercises that'll test our Kubernetes mettle. Every day brings a new challenge to conquer!
Code Snippet Stash: Forget cryptic incantations! Here, we'll store clear and concise code samples to illuminate the path forward.
Learnings Unleashed : No knowledge gets left behind! I'll document my understanding of each Kubernetes concept in clear, bite-sized chunks.


## Join the Mission! 

This odyssey isn't a solo trip! Whether you're a seasoned Kubernetes captain  or a curious space newbie , feel free to explore, contribute, and share your own insights. Together, let's conquer the vast Kubernetes frontier!

