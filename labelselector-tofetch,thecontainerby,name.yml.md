```bash
apiVersion: v1
kind: Pod
metadata:
  name: jspiders
  labels:
    department: DevOps
    batch: jddw3
spec:
  containers:
    - name: demo
      image: ubuntu
      command: ["/bin/bash", "-c", "while true; do echo hi everyone; sleep 5; done"]
```
