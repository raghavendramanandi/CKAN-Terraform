- This code can be used to deploy CKAN using terraform

Here some perspectives/vision and intentions from authors point:
- This is to be considered as the first iteration of provisioning CKAN using terraform
- I this first version, I have provisioned using shell scripts. I feel we would need to update some scripts to a more sophisticated techniques
- We should add a utility which would convert a template to an actual file. It will be very helpful in future
- Right now, the only as much code is written as required for basic provisioning.
- In the future, I would like to provision solr in a separate machine. PG in a separate instance.
- Restricting the security groups is of prime importance when we separate services to different boxes
- Auto-scaling groups for machine group
- I feel there are a few places when a custom AMI is more appropriate. Should address this at a logical point
- An AMI should be built for provisioning infra and services
- Rout53 for IP
- A provision to add custom services. Not sure how to do it. Need to figure out a way
- When we go for multi-instance CKAN servers, Authentication should be taken care
- Jenkins
  - Deployment
  - Build
- A data pipeline to load data into CKAN
- Data pipeline to be built on a DAG-based framework like airflow
- Automate admin user creation

Thanks to all the resource providers online
