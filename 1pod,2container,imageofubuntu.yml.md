```bash
apiVersion: v1
kind: Pod
metadata:
  name: flipkart
spec:
  containers:
    - name: login
      image: ubuntu
      command: ["/bin/bash", "-c", "while true; do echo hi everyone; sleep 5; done"]
    - name: qsp
      image: ubuntu
      command: ["/bin/bash", "-c", "while true; do echo hi everyone; sleep 5; done"]
  restartPolicy: Never     #Defaults to always
```
