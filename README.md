# roboshop-frontend

roboshop-frontend:
==================
kubectl exec -it frontend033nff -- bash
cat /etc/nginx
cat /etc/nginx/conf.d/default.conf
** after location paste "proxy "


argocd app --help ( to sync app automatically )
argocd app sync my-app(here my-app means frontend,cart,,.....)
