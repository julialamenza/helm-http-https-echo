This helm chart deploys the http-https-echo docker image to a kubernetes environment.

## Installing the chart

To install the chart with the release name my-release located in <chart-directory>:

``````
helm install --name my-release <chart-directory>
``````
This command deploys the chart with sane defaults.

A k8s service will be created with a ClusterIP configuration exposing two ports:

8080 -> HTTP
8443 -> HTTPs

### Uninstalling the Chart
To uninstall/delete the my-release deployment:

``````
helm delete my-release 
``````
