# jenkinscode
## kubernetes command that i know.
kubectl get namespace  //to see all namespaces in the cluster
kubectl get all -n namespace // to list all under a namespace
kubectl delete deployment deployment_name -n namespace //inorder to delete a deployment and start fresh
kubectl apply -f deployment.yaml // to deploy a deployment file
kubectl create namespace name // to create a namespace
kubectl delete namespace name // to delete a namspace
kubectl get deployment -n name -o yaml // to get the yaml file in the terminal
kubectl exec -it pod_name -n namepsace -- /bin/bash //to go inside the pod
kubectl exec -it pod_name -n namespace -- cat /var/lib/config.xml //to see the file in the terminal without going inside the pod
kubectl port-forward service/service_name 8081:8080 -n namepsace // port forwarding an application service(svc), here the app is deployed under 8080 and forwarding to 8081
kubectl get svc -n namespace //to list all services under a namespace
