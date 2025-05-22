# semana3.md

## 📅 Semana 3 – Segurança e Observabilidade

### Dia 11: RBAC básico
```yaml
yamls/role-rbac.yaml
```

### Dia 12-13: Prometheus + Grafana (via Helm)
```bash
helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
helm install prometheus prometheus-community/kube-prometheus-stack
```

### Dia 14: Network Policies
```yaml
apiVersion: networking.k8s.io/v1
kind: NetworkPolicy
metadata:
  name: deny-all
  namespace: dev
spec:
  podSelector: {}
  policyTypes:
  - Ingress
  - Egress
