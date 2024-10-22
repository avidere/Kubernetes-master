**To create hpa we need to follow below steps:**
- enable metriccs server to fetch metrics
- write hpa.yaml file and mention deployment name inside hpa file
- create deployment, service and hpa from yaml file
- create traffic generator from yaml file
- login to trafic generator pod and install wrk with command- apk add wrk
- execute command to generate load - wrk -c 5 -t 5 -d 300s -H "connection: close" http://utility-api-service:8080/api/stress

- ----------------------------------------------------------------------------------
**To create vpa( vertical pod auto scale).**
- install vpa on cluster from kubernetes git repositpry - https://github.com/kubernetes/autoscaler.git
**- install vpa by using command -**
- cd autoscaler
- ./vertical-pod-autoscaler/hack/vpa-up.sh"
- install execute vpa.yaml file

- --------------------------------------------------------------------------
To create cluster auto scale 
- install cluster autoscale on cluster from kubernetes git repositpry - https://github.com/kubernetes/autoscaler.git
**- install vpa by using command -**
- cd autoscaler
- ./vertical-pod-autoscaler/hack/vpa-up.sh"
- install execute vpa.yaml file
