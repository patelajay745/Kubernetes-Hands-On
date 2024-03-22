### you may never need to manipulate ReplicaSet objects: use a Deployment instead, and define your application in the spec section.

-----


#### You can remove Pods from a ReplicaSet by changing their labels. This technique may be used to remove Pods from service for debugging, data recovery, etc. Pods that are removed in this way will be replaced automatically ( assuming that the number of replicas is not also changed).

-----
