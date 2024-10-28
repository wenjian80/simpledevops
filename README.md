# simpledevops

No instruction yet. 

Go to src/app.yaml and replace it with your tenancy for your registry and your region.

Download the git as zip and copy to your cloud shell.

unzip the zip file.

Create the source reposiotry on oci devops and clone it your cloud shell using https.

copy those contents to your git and push those to oci devops soruce repository

```
git add -A
git commit -m "commit"
git push origin main
```

After deploy hit the below to get the service load balancer ip

The below command will show the load balancer ip as the external ip

```
kubectl get services

kubectl get services
NAME           TYPE           CLUSTER-IP     EXTERNAL-IP      PORT(S)             AGE
helloworldpy   LoadBalancer   10.96.89.168   xx.xx.xx.xxx   80:30915/TCP        7m43s
kubernetes     ClusterIP      10.96.0.1      <none>           443/TCP,12250/TCP   16h

```

And then hit the services
```
http://EXTERNAL-IP/
```