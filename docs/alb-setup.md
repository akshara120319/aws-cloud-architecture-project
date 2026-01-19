# Application Load Balancer (ALB) Setup

## Objective
To create an Application Load Balancer that distributes incoming traffic
across multiple EC2 instances to improve availability and performance.

## Steps Followed
1. Logged in to AWS Management Console.
2. Opened the EC2 service from the console.
3. Clicked on Load Balancers from the left menu.
4. Clicked on Create Load Balancer.
5. Selected Application Load Balancer.
6. Entered load balancer name as cloud-project-alb.
7. Selected Internet-facing scheme and IPv4.
8. Chose default VPC and selected two availability zones.
9. Created a new security group allowing HTTP (port 80).
10. Created a target group and registered EC2 instances.
11. Completed the setup and created the load balancer.

## Outcome
The Application Load Balancer was successfully created and became active.
