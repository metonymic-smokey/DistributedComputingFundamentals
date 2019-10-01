#Final Project Steps

1.Make sure your YAML files are in the same directory and run `minikube start`.

2.Create an NGINX pod using the `kubectl create` command.
The syntax is `kubectl create -f <YAML file name>`.     

The number of replicas given here is 2, it can be changed in the YAML to another number.  

3.Use `kubectl get pods` and `docker ps` to check for pod creation and container creatin respectively.

4.Now create a service, using a command similar to step 2.

5.Now run `kubectl get services` to check if the service is up and running.

6.Head to your browser and check `http://127.0.0.1:82` if you have used port 82.
Substitute with whichever port number you have used otherwise.

7.After completion of the project, `kubectl delete service <service-name>` and `kubectl delete rc <nameof replication controller>` can be used for deletion.

Note: Use your image from the previous week's assignment after pushing to Dockerhub if you want a custom page for NGINX.
