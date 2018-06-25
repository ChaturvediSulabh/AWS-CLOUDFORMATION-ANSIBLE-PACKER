# DevOps Assignment

Assignment 1
1. CloudformationscripttocreatebelowAWScomponents

• VPC with two public and private subnets
• Route tables for each subnet
• Security Group to allow port 80 and 443
• ELB and ALB
• Private route53 hosted zone and CNAME entry for both ALB and ELB
• S3 bucket
• IAM Policy for assignment-3
Delivery Outcome:
• Once Cloud formation script is executed, It will create a VPC with valid CIDR block, which contains all VPC related Resources such as valid subnets, route tables (public, private), security groups, NAT gateway, Internet Gateway etc.
• Also it will create AWS resources like Application load balancer and Elastic load balancer, and rout53 internal hosted zone
• DNS name will be created/ updated in Route 53 respectively ALB and ELB.
• IAM Role will be created, with right policy, which have proper S3 bucket access for EC2 servers and other resources related to question 3.
• Get all the Output details for every resources, in cloud formation Output Parameter.
Assignment 2
2. Ansible playbook to do following task
• Pick a Linux AMI
• Install webserver (Apache/Nginx)
• Download code from git
• Configure webserver with security best practices (List them)
• Create a self-signed certificate
• Secure a demo Wordpress site using self-signed certificate
Delivery Outcome:
• Choose any amazon machine image, install LAMP stack (Linux, Apache/ Nginx, mysql and PHP) from Ansible script
• Get the proper output from Ansibe modules to download the code from git (BitBucket/ GitHub), and update the server level securities.
• Use Ansible Modules for self-signed certificate, which will clearly reflect in Output.
• Wordpress site should be SSL enable and entry must be available in mysql database.
Assignment 3
2. ExecuteAnsibleplaybook
• Run Ansible playbook in a packer job and create AMI.

• Automatically create ASG using AMI created in output of assignment 2 and attach it to ELB.
• Showcase capability of ALB, by created two different domain route policy.
• Instance launched behind ELB/ALB should have role attached having access to s3 specific bucket, pull images from S3.
Delivery Outcome:
• Write a packer script to create AMI with above assignment.
• Execute another Ansible script in the same packer job, which can
create launch configuration (LC) and ASG attached the above AMI, this Launch configuration must be a part of Newly created Auto scaling group (AGS).
• Above created ALB is part of this Auto scaling Group, which can be redirect word press admin url to admin target group, and WordPress site url to public target group.
• IAM role created in Assignment 1, must be part of this auto scaling group, which have S3 bucket access and able to render the website images from S3 bucket.
Assignment 4
3. Createascriptusinganypreferredprogramminglanguage(python,Node.js, java etc.) to perform following activities
• List AWS services being used region wise
• List each service in detail, like EC2, RDS etc.
• Create AWS Code deploy, Application Group and Deployment Group
Delivery Outcome:
• Once script is executed user can save the output in text file, which have list of AWS resources and details of that resources region wise.
• Outcome of second script will create code deploy application group and deployment group.
