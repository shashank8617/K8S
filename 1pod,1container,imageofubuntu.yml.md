```bash
kind: pod
apiVersion: v1
metadata:
  name: jspiders
spec:
  containers:
    - name: jspiders
      image: ubuntu
      command: ["/bin/bash", "-c", "while true; do echo hi everyone; sleep 5; done"]
```
