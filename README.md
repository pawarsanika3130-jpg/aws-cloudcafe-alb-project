# Scalable Web Application with Application Load Balancer (ALB)

# Project Overview

This project demonstrates how to deploy a highly available web application on AWS using EC2 instances and an Application Load Balancer (ALB).

The ALB distributes incoming traffic across multiple EC2 instances and performs health checks to ensure users are always routed to healthy servers.
## AWS Services

- Amazon EC2
- Application Load Balancer (ALB)
- Target Groups
- Security Groups
- Amazon VPC
- Nginx Web Server

  ## Architecture

Internet Users
        ↓
Application Load Balancer
        ↓
 ┌───────────────┐
 │               │
 ▼               ▼
EC2-1         EC2-2
(Nginx)       (Nginx)

## Features

✔ Load Balancing

✔ High Availability

✔ Health Checks

✔ Automatic Failover

✔ Fault Tolerance

✔ Scalable Architecture
## Implementation Steps

1. Launch two EC2 instances
2. Install and configure Nginx
3. Create Target Group
4. Register EC2 instances
5. Configure Health Checks
6. Create Application Load Balancer
7. Route traffic to Target Group
8. Test load balancing
9. Simulate server failure
10. Verify automatic failover

    ## Results

- Traffic successfully distributed across two EC2 instances.
- ALB detected unhealthy targets automatically.
- Application remained available during server failure.
- Health checks restored traffic when server recovered.
