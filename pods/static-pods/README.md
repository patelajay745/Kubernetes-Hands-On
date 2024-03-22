### Static Pods are managed directly by the kubelet daemon on a specific node, without the API server observing them.
ssh my-node1
path  to put mainfests : /etc/kubernetes/manifests/

Change path of --pod-manifest-path=/etc/kubernetes/manifests/ in kubelet config

systemctl restart kubelet

crictl ps