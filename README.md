# Information-Repository
Testing purposes

```

References
http://odewahn.github.io/docker-jumpstart/building-images-with-dockerfiles.html
https://docs.docker.com/engine/reference/run/#name-name
https://www.digitalocean.com/community/tutorials/docker-explained-using-dockerfiles-to-automate-building-of-images
https://stackoverflow.com/questions/1559955/host-xxx-xx-xxx-xxx-is-not-allowed-to-connect-to-this-mysql-server
https://github.com/kubernetes/minikube/releases
http://192.168.1.33:8001/api/v1/namespaces/kube-system/services/http:kubernetes-dashboard:/proxy/#!/overview?namespace=default

Docker build images
$ docker build -t "simple_flask:dockerfile" .

Docker run images (+creates containers)
$ docker run --name [image name] -e AUTHOR="[username]" -d -P [repo-name/image-name]

Docker ports (where containers are hosted)
$ docker ports [image name]

Exporting from Docker
$ docker exec -it database-service mysqldump -p -uroot -ppassword db_drupal > drupal.sql


# remove the token ...
KUBE_EDITOR="nano" kubectl edit secret $(kubectl get secrets --namespace=kube-system -o jsonpath='{.items[0].metadata.name}') --namespace=kube-system

# get pods
kubectl get pods --all-namespaces


1. Install Docker
2. Install Composer
3. Install Kubernetes (minikube for local installation)


https://wadatabase.azurewebsites.net/
https://wasolrservice.azurewebsites.net
https://waquerytoolservice.azurewebsites.net
https://wadrupalservice.azurewebsites.net


kubectl proxy &
ssh -R 30000:127.0.0.1:8001 $USER@192.168.0.20
http://192.168.0.20:30000




https://www.techrepublic.com/article/how-to-quickly-install-kubernetes-on-ubuntu/
https://kubernetes.io/docs/setup/independent/create-cluster-kubeadm/
```


Please view the Wiki for this project
https://github.com/Services-Sandbox/Information-Repository/wiki

kubectl create clusterrolebinding cluster-system-anonymous --clusterrole=cluster-admin --user=system:anonymous



