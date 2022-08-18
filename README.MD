This repo contains Flask app deployment configs for Kubernetes:

Steps to deploy:
1. Run "kubectl apply -f namespace_volume.yaml"
2.a If you want classic deployment with persistent volume - run "kubectl apply -f mysql_deployment.yaml"
2.b If you want deploy mysql as Statefulset - run "kubectl apply -f mysql_statefulset.yaml"
3. Run Flask app with "kubectl apply -f flask-app-deployment.yaml" 