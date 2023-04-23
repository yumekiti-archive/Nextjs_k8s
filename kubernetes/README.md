```
argocd app create \
  nextjs-app \
  --repo https://github.com/yumekiti/Nextjs_k8s \
  --path kubernetes \
  --dest-server https://kubernetes.default.svc \
  --dest-namespace default \
  --sync-policy automated \
  --auto-sync \
  --auto-prune \
  --self-heal
```