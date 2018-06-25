# DevOps Assignment

## Assignment 1 [Click Here to go-to Solution](Assignment-1)
1. CloudformationscripttocreatebelowAWScomponents

- [x] VPC with two public and private subnets
- [x] Route tables for each subnet
- [x] Security Group to allow port 80 and 443
- [x] ELB and ALB
- [x] Private route53 hosted zone and CNAME entry for both ALB and ELB
- [x] S3 bucket
- [x] IAM Policy for assignment-3
#### Delivery Outcome:
- [x] Once Cloud formation script is executed, It will create a VPC with valid CIDR block, which contains all VPC related Resources such as valid subnets, route tables (public, private), security groups, NAT gateway, Internet Gateway etc.
- [x] Also it will create AWS resources like Application load balancer and Elastic load balancer, and rout53 internal hosted zone
- [x] DNS name will be created/ updated in Route 53 respectively ALB and ELB.
- [x] IAM Role will be created, with right policy, which have proper S3 bucket access for EC2 servers and other resources related to question 3.
- [x] Get all the Output details for every resources, in cloud formation Output Parameter.

## Assignment 2 [Click Here to go-to Solution](Assignment-2)
2. Ansible playbook to do following task

- [x] Pick a Linux AMI
- [x] Install webserver (Apache/Nginx)
- [x] Download code from git
- [x] Configure webserver with security best practices (List them)
- [x] Create a self-signed certificate
- [x] Secure a demo Wordpress site using self-signed certificate
#### Delivery Outcome:
- [x] Choose any amazon machine image, install LAMP stack (Linux, Apache/ Nginx, mysql and PHP) from Ansible script
- [x] Get the proper output from Ansibe modules to download the code from git (BitBucket/ GitHub), and update the server level securities.
- [x] Use Ansible Modules for self-signed certificate, which will clearly reflect in Output.
- [x] Wordpress site should be SSL enable and entry must be available in mysql database.
## Assignment 3 [Click Here to go-to Solution](Assignment-3)
3. ExecuteAnsibleplaybook

- [x] Run Ansible playbook in a packer job and create AMI.
- [x] Automatically create ASG using AMI created in output of assignment 2 and attach it to ELB.
- [x] Showcase capability of ALB, by created two different domain route policy.
- [x] Instance launched behind ELB/ALB should have role attached having access to s3 specific bucket, pull images from S3.
#### Delivery Outcome:
- [x] Write a packer script to create AMI with above assignment.
- [x] Execute another Ansible script in the same packer job, which can
create launch configuration (LC) and ASG attached the above AMI, this Launch configuration must be a part of Newly created Auto scaling group (AGS).
- [x] Above created ALB is part of this Auto scaling Group, which can be redirect word press admin url to admin target group, and WordPress site url to public target group.
- [x] IAM role created in Assignment 1, must be part of this auto scaling group, which have S3 bucket access and able to render the website images from S3 bucket.
## Assignment 4 [Click Here to go-to Solution](Assignment-4)
3. Createascriptusinganypreferredprogramminglanguage(python,Node.js, java etc.) to perform following activities

- [x] List AWS services being used region wise
- [x] List each service in detail, like EC2, RDS etc.
- [x] Create AWS Code deploy, Application Group and Deployment Group
#### Delivery Outcome:
- [x] Once script is executed user can save the output in text file, which have list of AWS resources and details of that resources region wise.
- [x] Outcome of second script will create code deploy application group and deployment group.
