# Highly Available Cloud Web Application on AWS

## About the Project
This project is a cloud-based web application architecture built using AWS services.
The main idea of this project is to understand how real applications are deployed on
cloud infrastructure with proper security, scalability, and monitoring.

This project is completely cloud-focused. 
The entire work is done using core AWS services and cloud concepts.

## Why I Chose This Project
I wanted to work on a project that helps me understand real-world cloud architecture.
Instead of focusing on coding, this project helped me learn how applications are
actually hosted, scaled, secured, and monitored on cloud platforms like AWs.

## AWS Services Used
- EC2 for running application servers
- Application Load Balancer to distribute traffic
- Auto Scaling Group for handling traffic changes
- VPC for network isolation
- Public and Private Subnets
- Security Groups for access control
- IAM for user and role management
- S3 for storing files and backups
- RDS for database service
- Lambda for serverless background tasks
- CloudWatch for monitoring and logs

## Architecture Diagram
![AWS Architecture](aws-architecture.png.png)

## Architecture Explanation
When a user accesses the application, the request first reaches the Application Load
Balancer. The Load Balancer distributes the traffic to EC2 instances running inside
private subnets.

Auto Scaling Group automatically increases or decreases EC2 instances based on load.
The application data is stored in an RDS database which is also placed in a private
subnet for security. Static files and backups are stored in Amazon S3.

AWS Lambda is used for background tasks such as processing events or scheduled jobs.
CloudWatch is used to monitor performance, logs, and system health.

This setup provides high availability, scalability, and security.

## VPC and Networking
A custom VPC is created for this project.
- Public subnets are used for the Load Balancer
- Private subnets are used for EC2 instances and RDS
- Internet Gateway allows users to access the application
- Route Tables manage traffic flow

This networking setup keeps backend resources secure and isolated.

## Scalability and Availability
Auto Scaling Group is configured to handle traffic automatically.
When traffic increases, new EC2 instances are launched.
When traffic decreases, extra instances are terminated.

Application Load Balancer ensures traffic is evenly distributed
and the application remains available even if one instance fails.

## Security Implementation
Security is handled using AWS best practices:
- EC2 instances are not directly accessible from the internet
- RDS database is accessible only from EC2 instances
- Security Groups allow limited and required traffic only
- IAM roles are used instead of hard-coded credentials

## Storage and Database
Amazon S3 is used to store static files and backup data.
Amazon RDS is used as a managed relational database service.
The database is deployed in a private subnet to improve security.

## Serverless Usage
AWS Lambda is used for:
- Event-based tasks
- Background processing
- Reducing the need for additional servers

## Monitoring and Logging
AWS CloudWatch is used to:
- Monitor EC2 CPU usage
- Track Auto Scaling activity
- Store application and Lambda logs
- Create alarms for high resource usage

## AWS Console Screenshots

### EC2 Instances
![EC2](aws%20screenshort/ec2.png)

### Application Load Balancer
![ALB](screenshots/alb.png)

### Auto Scaling Group
![AutoScaling](auto scalting.png)

### S3 Bucket
![S3](screenshots/s3.png)

### RDS Database
![RDS](screenshots/rds.png)

### CloudWatch Monitoring
![CloudWatch](screenshots/cloudwatch.png)

## What I Learned from This Project
- How real cloud architecture works
- How applications are scaled on AWS
- How security is managed in cloud networks
- How monitoring helps in maintaining system health

## Conclusion
This project helped me gain practical experience in cloud computing.
I now have a clear understanding of how real-world applications are deployed
and managed using AWS cloud services.

Akshara Joshi  
Final Year B.Tech (CSE – AI & ML)
Cloud Computing Enthusiast
