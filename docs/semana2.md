# semana2.md

## 📅 Semana 2 – Configurações e Volumes

### Dia 6: ConfigMaps e Secrets
```yaml
yamls/configmap.yaml
yamls/secret.yaml
```

### Dia 7: Volumes
- [ ] Criar volume `emptyDir` e montar em container

### Dia 8-9: Health checks
```yaml
livenessProbe:
  httpGet:
    path: /
    port: 80
  initialDelaySeconds: 5
  periodSeconds: 10
```

### Dia 10: Rolling Updates
```bash
kubectl rollout status deployment nginx-deployment
kubectl rollout undo deployment nginx-deployment
