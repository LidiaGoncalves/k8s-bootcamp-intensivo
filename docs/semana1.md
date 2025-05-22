# semana1.md

## 📅 Semana 1 – Fundamentos e Primeiros Deploys

### Dia 1: Conceitos Essenciais
- [ ] O que é Kubernetes? (Leia: https://kubernetes.io/docs/concepts/overview/)
- [ ] Componentes principais do cluster
- [ ] Objetos principais: Pod, ReplicaSet, Deployment, Service

### Dia 2: Setup local
- [ ] Instalar Minikube ou Kind
- [ ] Rodar seu primeiro cluster local:
```bash
minikube start
kubectl get nodes
```

### Dia 3: Criar Pods e Deployments
```yaml
yamls/nginx-pod.yaml
yamls/nginx-deployment.yaml
```

### Dia 4: Services e Exposição
```yaml
yamls/nginx-service.yaml
```

### Dia 5: Namespaces e Debugging
```bash
kubectl create namespace dev
kubectl get pods -n dev
kubectl logs <pod>
kubectl describe pod <pod>
kubectl exec -it <pod> -- /bin/bash
```

---
