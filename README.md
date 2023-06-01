# History Spinnaker
Development Started in 2014 by Netflix
Netflix start using it in 2015 in their production development.
Open-sourced in 2015 November
Now it uses by Netflix, Google, Microsoft, Veritas, Target, Kenzen etc.

# What is Spinnaker?
Spinnaker is an open-source continuous delivery platform designed for deploying and  managing applications in cloud environments
## Multi-Cloud Deployment: 
Spinnaker supports deployment across multiple cloud providers, including AWS, Azure, Google Cloud, and Kubernetes.
</br>
## Continuous Delivery:
Spinnaker enables teams to automate the application release process, allowing for frequent and reliable deployments.

## Deployment Strategies: 
It provides various deployment strategies such as blue/green(The blue environment represents the current production environment running the existing version of the application, while the green environment represents the new version of the application.), canary, rolling updates, and more, allowing for controlled and low-risk deployments.
Spinnaker Support all the Major cloud providers.
Create pipelines that run integration and System test with Trigger via git event,  Jenkins, Travis CI, Docker, Cron, and others.


# Spinnaker features
![Screenshot from 2023-05-29 10-28-57](https://github.com/aadilraza339/spinnaker-deployment/assets/47937273/75c6a0ee-8eec-4829-b9da-addbed8a36cb)

### Multi-cloud deployment

It supports cloud platforms such as AWS, Azure, GCP, Oracle Cloud, Cloud Foundry, and OpenStack.

### CI integrations
Spinnaker’s robust and automated release pipelines can be easily integrated with other tools such as:
Jenkins
Travis CI
Git event
CRON jobs

### Monitoring & notification integrations
Spinnaker can be easily integrated with monitoring solutions such as Datadog, Prometheus, SignalFx, and Stackdriver for metrics collection and analysis.

### Support for different deployment strategies
Deploy faster with easier rollbacks
Handle config drift issues much more effectively.

### Let’s look at each step of the workflow:
Developers commit/push code to a centralized repository.
The completed code triggers Jenkins to test and build a container.
This container gets pushed to a container registry.
The spinnaker listens for a new image in the container registry and triggers the delivery pipeline for deployment.
The Spinnaker pipeline creates the necessary configurations (application configs, instances, scaling, etc.) and deploys the container in a target Kubernetes cluster after manual review.
