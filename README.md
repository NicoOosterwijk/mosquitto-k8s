# Mosquitto kustomization K8s

```
apiVersion: fleet.cattle.io/v1alpha1
kind: GitRepo
metadata:
  name: mosquitto
  namespace: fleet-default
  labels:
    mosquitto: enabled
spec:
  branch: main
  repo: https://github.com/NicoOosterwijk/mosquitto-k8s.git
  targets:
    - clusterGroup: mosquitto
```