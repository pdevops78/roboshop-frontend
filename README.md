# roboshop-frontend

roboshop-frontend:
==================
kubectl exec -it frontend033nff -- bash
cat /etc/nginx
cat /etc/nginx/conf.d/default.conf
** after location paste "proxy "


argocd app --help ( to sync app automatically )
argocd app sync my-app(here my-app means frontend,cart,,.....)


eks jobs:
=========
kubernetes jobs :
==================
** one image can run multiple tasks is called jobs in eks.


apiVersion: batch/v1
kind: Job
metadata:
metadata:
    name: {{ .Values.component }}
    namespace: argocd
    labels:
    appName: {{ .Values.labels.appName }}
    project_Name: {{ .Chart.name }}
spec:
template:
spec:
containers:
- name: schema
  image:  pavanidevops78/kubernetes:{{ .Values.schema.schema_imageVersion }}
restartPolicy: Never
backoffLimit: 1


* docker run -it docker.io/redhat/ubi9
  vi /etc/yum.repos.d/mongo.repo
  2   yum install -y mongodb-org
  3  dnf list all | grep mongo
  4  dnf install mongodb-mongosh.x86_64 -y
  5  mongosh
  6  mongosh --version
* mongosh --help
* 


