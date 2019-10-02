# Final Project Steps

1.Make sure your YAML files are in the same directory and run `minikube start`.   

2.Create an NGINX pod using the `kubectl create` command.    
The syntax is `kubectl create -f <YAML file name>`.         

The number of replicas given here is 2, it can be changed in the YAML to another number.      

3.Use `kubectl get pods` and `docker ps` to check for pod creation and container creatin respectively.    

4.Now create a service, using a command similar to step 2.   

5.Now run `kubectl get services` to check if the service is up and running.   
The External IP  column there can take some time to appear so keep re trying this command.

6.After completion of the project, `kubectl delete service <service-name>` and `kubectl delete rc <nameof replication controller>` can be used for deletion.   

Note: Use your image from the previous week's assignment after pushing to Dockerhub if you want a custom page for NGINX. 

Check this link out: http://containertutorials.com/get_started_kubernetes/k8s_example.html
