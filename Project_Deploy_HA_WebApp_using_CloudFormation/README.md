Deploy a High-Availability Web App using CloudFormation

Order of execution:
1. Create stack with network.yml and network-params.json (using the create.sh -> ./create.sh network-stack ./network.yml ./network-params.json)
2. Create stack with server.yml and server-params.json (using the create.sh bash script -> ./create.sh server-stack ./server.yml ./server-params.json)

Parameters:
EnvironmentName should match in both network and server parameters.
AMItoUse in server-params.json should be Linux 18 as requested from the requirements. I have currently chosen AMI from us-east-1 that is Linux 18.
BucketName is the name of the bucket where the index.html file should be present.

The current index.html has the following as it's content.
<html>
<h1>it works! Udagram, Udacity</h1>
</html>