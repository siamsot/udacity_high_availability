#General info

In this repository, we have a script for AWS CloudFormation which deploys an app in a VPC which has 2 private networks and 2 public along with a Load Balancer. In those networks, we deploy 2 EC2 instances for resilience. 

##Infrastructure

The script creates 2 subnets with an Internet Gateway along with a Load Balancer. The app that gets deployed on the EC2 instances which are in a separate subnet is from a S3 bucket so the IAM permissions are also created and given to the instances in order to be able to download the app.

## Diagram

![template1-designer (1)](https://user-images.githubusercontent.com/22414982/109536931-9b21f180-7abe-11eb-9694-f2e12866da93.png)


The script was developed as an excersise for the Udacity DevOps Nanodegree.
