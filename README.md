# Launching-an-EKS-Cluster

    Elastic Kubernetes Service (EKS) is a fully managed Kubernetes service from AWS. In this lab, you will work with the AWS command line interface and console, 

    using command line utilities like eksctl and kubectl to launch an EKS cluster, provision a Kubernetes deployment and pod running instances of nginx, 
    
    and create a LoadBalancer service to expose your application over the internet.
    
    
 - Create an IAM User with Admin Permissions
    
    Create an IAM user with programmatic access and administrator-level privileges.
    
    aws console > services > IAM > user > create user > programmatic access > attach existing policy directly > select AdministratorAccess > 
    
    Take note of the access key and secret access key of your user because we will use them in the next step.
    
    
- Launch an EC2 Instance and Configure the Command Line Tools
    
    Create an EC2 instance in us-east-1 region. 
    
    select Auto assign public ip when creating ec2 instance > rest all defaults > download key pair
    
    
    If necessary, upgrade the AWS CLI on your EC2 instance to CLI v.2x or later.
    
    Configure the AWS CLI using the credentials of the user you just created.
    
    Install eksctl on your EC2 instance.
    
    Install kubectl on your EC2 instance.


- Provision an EKS Cluster

    Use eksctl to provision an EKS cluster with three worker nodes in us-east-1.
    
    Use Kubernetes version 1.16 or later.
       
    
- Create a Deployment on Your EKS Cluster     
    
    Use kubectl to create a LoadBalancer service.
    
    Check the status of your LoadBalancer service using kubectl.
    
    Use kubectl to create a Deployment on your EKS cluster, using the standard nginx image EKS has available in the default Docker Hub registry.
    
    Check the status of your cluster, deployment, and pods using kubectl.
    
    When the Deployment is up and running, check that you can access your application using the DNS name of the LoadBalan


- Test the High Availability Features of Your EKS Cluster 

    In the AWS Console, shut down all the worker nodes.
    
    Check the status of your cluster, deployment, and pods using kubectl.
    
    After a few minutes, you should see EKS launching new instances to keep your service running.
    
    When the cluster is back to a steady state, check that your application is up and running.





    
    
    
    
