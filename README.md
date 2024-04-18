Run the app in Kubernetes

The folder Sample-voting-app contains the YAML specifications of the Voting App's services.

Run the following command to create the deployments and services. Note it will create these resources in your current namespace (default if you haven't changed it.)

kubectl create -f Sample-voting-app/
The vote web app is then available on port 30100 on each host of the cluster, the result web app is available on port 30200.

To remove them, run:

kubectl delete -f Sample-voting-app/
