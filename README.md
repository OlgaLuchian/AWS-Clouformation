# aws-clouformation

![Alt text](images/logo.png?raw=true "Title")


## What is AWS CloudFormation?

AWS CloudFormation is a service that gives developers and businesses an easy way to create a collection of related AWS and third party resources and provision them in an orderly and predictable fashion.


[Official Documentation Link](https://aws.amazon.com/cloudformation/#:~:text=AWS%20Cloud%E2%80%8BFormation&text=AWS%20CloudFormation%20allows%20you%20to,AWS%20and%20third%20party%20resources)

## Templates

* [s3bucket.yaml](s3bucket.yaml)

This template will provision S3 bucket with tags applied and versioning enabled.

* [security_group.yaml](security_group.yaml)

This template will create a security group with tags applied and will allow https only.

* [ec2_instance.yaml](ec2_instance.yaml)

This template will create an EC2 Instance with the following properties:  

    - t2.micro
    - Encrypted EBS volume
    - Tags applied

* [ec2_parameter_instance.yaml](ec2_parameter_instance.yaml)

This template will create an EC2 Instance using parameters to pass values to the template when creating or updating a stack so that you can customize each stack deployment. Provide the following values for the template.

    - EC2 Type   
    - Subnet ID
    - AMI
    - SSH KEY
    - Security Group
    - Team 
    - Owner
    - Volume size

