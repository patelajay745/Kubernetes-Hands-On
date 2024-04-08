## HorizontalPodAutoscaler

To create the horizontalpodautoscaler

`kubectl autoscale deployment ele-ecommerce --cpu-percent=50 --min=1 --max=10`

`kubectl get hpa`

To increase load to test:

`kubectl run -i --tty load-generator --rm --image=busybox:1.28 --restart=Never -- /bin/sh -c "while sleep 0.01; do wget -q -O- http://php-apache; done"
`
