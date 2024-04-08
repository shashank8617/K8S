```bash
apiversion: v1
kind: ReplicationController
metadata:
  name: flipkart
spec:
  replicas: 2
  selector:
    app: nginx
  template:
    metadata:
      name: signup
      labels:
        app: nginx
    spec:
      containers:
        - name: signupemail
          image: nginx
          ports:
          - containersPort: 80
```
