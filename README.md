# Branch for Files Mock Test Answer
To see the list of files for mock test answer, go to "master" branch.

# Answer for Mock Test:

# Question 1
- Create new namespace: kubectl create namespace qq2
- Run command : kubectl apply -n qq2 -f deployment_nginx.yaml

# Question 2
- Run command: kubectl apply -n qq2 -f lab_deployment.yaml
- To scale deployment into 4 replicas: kubectl scale deployment lab-deployment --replicas=4 -n qq2

# Question 3
- To create new namespace: kubectl create namespace qq3
- Create a deployment names nginx-deployment: kubectl create deployment nginx-deployment --image=nginx:nginx -n qq3
- Perform a rolling update to the deployment: kubectl set image deployment nginx-deployment nginx=alpine -n qq3
- To check: kubectl describe deployment nginx-deployment -n qq3

# Question 4
- Run commnad: kubectl apply -n qq3 -f apache_deployment.yaml
- To check the deployment: kubectl describe deployment apache-deploymeht -n qq3
- Perform rolling update to the image: kubectl set image deployment apache-deploymeht apache=httpd:bookworm -n qq3
- rollback of the deployment: kubectl rollout undo deployments/apache-deploymeht -n qq3

# Question 5
- Create configmap: kubectl apply -f configMap.yaml
- Create secret: kubectl apply -f secret.yaml
- Apply deployment: kubectl apply -f apache_pod.yaml

# Question 6
- create daemonset: kubectl apply -f daemon_set.yaml -n qq3

# Question 7
- Create limit: kubectl apply -n qq3 -f pod_limit.yaml

# Question 8
- Apply deployment with service: kubectl apply -n ca1 -f ingress_deployment.yaml
- Create ingress: kubectl apply -n ca1 -f ingress.yaml
  
# Question 9
- Create a new Deployment named app01: kubectl apply -f app01-deployment.yaml -n prod
- Create a new Service named app01-svc: kubectl apply -f app01-svc.yaml -n prod







