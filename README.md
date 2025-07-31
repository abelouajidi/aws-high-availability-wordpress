# aws-high-availability-wordpress
High-Availability WordPress with RDS and EFS


AWS High-Availability WordPress

    A fully high-availability WordPress deployment on AWS using:
    
    Amazon EC2 in an Auto Scaling Group
    
    Application Load Balancer for traffic distribution
    
    Amazon EFS for shared storage of WordPress uploads
    
    Amazon RDS (MySQL) for managed database hosting
    
    Multi-AZ architecture for fault tolerance and scalability
    

📌 Architecture Overview

    [User Browser]
           |
    [Amazon Route 53]
           |
    [Application Load Balancer]
           |
    [Auto Scaling Group of EC2s]
           |
    [Amazon EFS] — shared uploads directory
           |
    [Amazon RDS - MySQL] — WordPress DB
    
🎯 Objectives

    - Build a fault-tolerant WordPress site across multiple Availability Zones
    - Use EFS to store uploads so all EC2 instances share the same content
    - Use RDS Multi-AZ for a highly available database
    - Deploy EC2 instances using Auto Scaling Groups
    - Configure a custom domain with Route 53

🛠 AWS Services Used

    - VPC	Isolated network for application
    - EC2	Hosts WordPress application
    - Auto Scaling	Automatically adjusts instance count
    - Application Load Balancer	Distributes HTTP/HTTPS traffic
    - EFS	Shared filesystem for WordPress media
    - RDS (MySQL)	Managed WordPress database
    - Route 53	Domain and DNS management
    - IAM	Permissions and security
    - CloudWatch	Monitoring and alerts
