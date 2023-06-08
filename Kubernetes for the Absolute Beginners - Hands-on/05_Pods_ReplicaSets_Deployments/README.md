## Section 05: Kubernets Concepts: Pods ReplicaSets Deployments

#### Table of Contents
- Pods with YAML
- Demo - Pods with YAML
- Tips & Tricks - Developing Kubernetes Manifest files with Visual Studio Code
- Hands-On Labs - Familiarise with the lab environment
- Hands-On Labs
- Solution : Pods with YAML Lab
- Replication Controllers and ReplicaSets
- Demo - ReplicaSets
- Hands-On Labs
- Solution - ReplicaSets
- Deployments
- Demo - Deployments
- Hands-On Labs
- Solution - Deployments
- Deployments - Update and Rollback
- Demo - Deployments - Update and Rollback
- Lab: Practice Test Rolling Updates and Rollbacks
- Solution - Rolling Updates and Rollbacks
- Coding Exercise 01: Pods - 1
- Coding Exercise 02: Pods - 2
- Coding Exercise 03: Pods - 3
- Coding Exercise 04: Pods - 4
- Coding Exercise 11: Pods - 5
- Coding Exercise 05: Pods - 6
- Coding Exercise 06: Pods - 7
- Coding Exercise 07: Pods - 8
- Coding Exercise 08: Pods - 9
- Coding Exercise 09: ReplicaSet - 1
- Coding Exercise 10: ReplicaSet - 2
- Coding Exercise 12: ReplicaSet - 3
- Coding Exercise 13: ReplicaSet - 4
- Coding Exercise 14: ReplicaSet - 5
- Coding Exercise 15: ReplicaSet - 6
- Coding Exercise 16: ReplicaSet - 7
- Coding Exercise 17: Deployment - 1
- Coding Exercise 18: Deployment - 2
- Coding Exercise 19: Deployment - 3
- Coding Exercise 20: Deployment - 4
- Coding Exercise 21: Deployment - 5
- Coding Exercise 22: Deployment - 6
- Coding Exercise 23: Deployment - 7



### Pods with YAML

#### YAML in Kubernetes
`pod-definition.yml`
```yaml
apiVersion: v1
kind: Pod
metadata:
  name: myapp-pod
  labels:
    app: myapp
    type: front-end
spec:
  containers:
    - name: nginx-container
      image: nginx
```

| **Kind**   | **Version** |
|------------|-------------|
| POD        | v1          |
| Service    | v1          |
| ReplicaSet | apps/v1     |
| Deployment | apps/v1     |

#### Kubectl Commands
```
kubectl create -f pod-definition.yml
kubectl get pods
kubectl describe pod myapp-pod
```


### Demo - Pods with YAML
```
vim pod.yml
```

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: nginx
  labels:
    app: nginx
    tier: frontend
spec:
  containers:
    - name: nginx-container
      image: nginx
```

#### Kubectl Commands
```
kubectl apply -f pod.yaml
kubectl get pods
kubectl describe pod nginx
```



### Tips & Tricks - Developing Kubernetes Manifest files with Visual Studio Code

IDE: [Visual Studio Code](https://code.visualstudio.com/)

Install extension: YAML -> Extension Settings -> Yaml: Schemas -> Edit in `settings.json`

Alternative: Ctrl + P -> Type "settings.json" 

```json
{
  "yaml.schemas": {
    "kubernetes": "*.yaml"
  }
}
```


### Hands-On Labs - Familiarise with the lab environment




### Hands-On Labs




### Solution : Pods with YAML Lab




### Replication Controllers and ReplicaSets




### Demo - ReplicaSets




### Hands-On Labs




### Solution - ReplicaSets




### Deployments




### Demo - Deployments




### Hands-On Labs




### Solution - Deployments




### Deployments - Update and Rollback




### Demo - Deployments - Update and Rollback




### Lab: Practice Test Rolling Updates and Rollbacks




### Solution - Rolling Updates and Rollbacks




### Coding Exercise 01: Pods - 1




### Coding Exercise 02: Pods - 2




### Coding Exercise 03: Pods - 3




### Coding Exercise 04: Pods - 4




### Coding Exercise 11: Pods - 5




### Coding Exercise 05: Pods - 6




### Coding Exercise 06: Pods - 7




### Coding Exercise 07: Pods - 8




### Coding Exercise 08: Pods - 9




### Coding Exercise 09: ReplicaSet - 1




### Coding Exercise 10: ReplicaSet - 2




### Coding Exercise 12: ReplicaSet - 3




### Coding Exercise 13: ReplicaSet - 4




### Coding Exercise 14: ReplicaSet - 5




### Coding Exercise 15: ReplicaSet - 6




### Coding Exercise 16: ReplicaSet - 7




### Coding Exercise 17: Deployment - 1




### Coding Exercise 18: Deployment - 2




### Coding Exercise 19: Deployment - 3




### Coding Exercise 20: Deployment - 4




### Coding Exercise 21: Deployment - 5




### Coding Exercise 22: Deployment - 6




### Coding Exercise 23: Deployment - 7




