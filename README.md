kind: Service
metadata:
name: web-app-01
labels:
app: web-app
selector:
app: web-app
version: v1.0.0
kind: Deployment
metadata:
name: web-app-01
spec:
template:
metadata:
labels:
app: web-app
version: "v1.0.0"


kind: Service
metadata:
name: web-app-02
labels:
app: web-app
selector:
app: web-app
version: v2.0.0


kind: Deployment
metadata:
name: web-app-02
spec:
template:
metadata:
labels:
app: web-app
version: "v2.0.0"
