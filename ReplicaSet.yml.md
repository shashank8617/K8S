```bash
apiVersion: v1
kind: ReplicaSet
metadata:
  name: jsp
spec:
  replicas: 2
  selector:
    matchExpressions:
    - {key: myname, operator: In, values: [qspider, jspider, pyspider]}
    - {key: env, operator: NotIn, values: [skillnary]}
  template:
    metadata:
      name: sak
      labels:
        myname: qspider
    spec:
      containers:
        - name: abc
          image: ubuntu
          command: ["/bin/bash", "-c", "while true; do echo hello world; sleep 3; done"]
```
