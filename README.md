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

    - EC2 Type          EC2-Instance Type
    - Subnet ID         SubnetId to which the EC2 should be launched
    - AMI               Amazon Image ID
    - SSH KEY           SSH Key name for SSH Access
    - Security Group
    - Team Tag          Value for Team Tag key
    - Owner             
    - Root Volume size  Size of the root volume

* [ec2_sg.yaml](ec2_sg.yaml)

CloudFormation Template that creates EC2-Instance and Security Group with Tags, and requires the following parameteres.

* [myvpc.yaml](myvpc.yaml)

CloudFormation Template will create the following resources:

    - Internet Gateway
    - VPC
    - Gateway Attachment
    - Subnet 1
    - Subnet 2
    - Route Table
    - Route 
    - Subnet Route Table Association 1
    - Subnet Route Table Association 2


It will take inputs from the following parameters:

    - Team Tag Value
    - Env Tag Value
    - Subnet 1 Cidr Block
    - Subnet 2 Cidr Block



Note: modify the file with your inputs.



