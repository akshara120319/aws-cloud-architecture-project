# Auto Scaling Group Setup

## Objective
To automatically increase or decrease the number of EC2 instances
based on application load.

## Steps Followed
1. Opened EC2 service in AWS Console.
2. Created a Launch Template with Amazon Linux 2 AMI.
3. Selected t2.micro instance type.
4. Attached the required security group.
5. Created an Auto Scaling Group using the launch template.
6. Selected default VPC and multiple subnets.
7. Attached the Auto Scaling Group to the existing Application Load Balancer.
8. Set minimum capacity as 1, desired capacity as 1, and maximum capacity as 2.
9. Created the Auto Scaling Group.

## Outcome
Auto Scaling Group was successfully created and is managing EC2 instances
based on defined capacity.
