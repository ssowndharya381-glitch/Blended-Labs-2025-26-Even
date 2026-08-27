# Lab 6 – Scale and Load Balance Your Architecture

## Title

Scale and Load Balance Your Architecture
Author :  
your name: SOWNDHARYA S  
Reg no :212225220100  
Date :27-08-2026  


## Objective

The objective of this lab is to understand how to design a scalable and highly available architecture on AWS using Auto Scaling and Elastic Load Balancing. This experiment focuses on distributing incoming traffic across multiple EC2 instances, automatically scaling resources based on demand, and validating fault tolerance.

## Prerequisites

* Basic knowledge of Amazon EC2 and VPC
* Completion of previous labs (IAM, EC2, EBS, Database Server)
* AWS Academy Lab access
* Stable internet connection

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Elastic Load Balancer (ELB / ALB)
* Auto Scaling Groups (ASG)
* Amazon CloudWatch

---

## Tasks Performed

### Task 1: Review Existing Architecture

Students review the existing EC2-based application architecture created in previous experiments.

### Task 2: Create a Launch Template

Students create a launch template that defines the EC2 instance configuration including AMI, instance type, security group, and user data.

### Task 3: Create an Auto Scaling Group

Students create an Auto Scaling Group using the launch template and configure minimum, maximum, and desired instance capacity.

### Task 4: Configure an Application Load Balancer

Students create an Application Load Balancer and configure target groups for routing traffic to EC2 instances.

### Task 5: Register Auto Scaling Group with Load Balancer

Students attach the Auto Scaling Group to the target group of the load balancer.

### Task 6: Configure Scaling Policies

Students configure scaling policies based on CPU utilization using Amazon CloudWatch alarms.

### Task 7: Test Load Balancing and Scaling

Students test the setup by generating traffic and observing automatic scaling and load distribution.


## Workflow (To be filled by Student)
Open the AWS Management Console and navigate to the Amazon EC2 service.
Explore the EC2 dashboard and check Instances, AMIs, Instance Types, Key Pairs, and Security Groups.
Launch a new EC2 instance using the Amazon Linux 2 AMI and select the t2.micro instance type.
Provide an instance name, select/create a Key Pair, and configure a Security Group.
Allow SSH (Port 22) access from the required IP address and HTTP (Port 80) access from anywhere.
Launch the instance and wait until the Instance State becomes Running and the status checks are completed.

## Output Screenshots 
<img width="673" height="328" alt="Screenshot 2026-08-27 095816" src="https://github.com/user-attachments/assets/52488bcf-19bb-4e26-972e-3195c67ac41c" />
<img width="674" height="320" alt="Screenshot 2026-08-27 095836" src="https://github.com/user-attachments/assets/8205beb9-0e77-49b2-a90e-72b151b7b5e8" />
<img width="676" height="326" alt="Screenshot 2026-08-27 095852" src="https://github.com/user-attachments/assets/f6a82ff3-4427-49ad-bc97-48bac2d25974" />


## Result

This experiment demonstrated how to build a scalable and fault-tolerant cloud architecture using Auto Scaling Groups and Elastic Load Balancing. The system automatically adjusted resources based on workload and ensured continuous service availability by distributing traffic across multiple instances.
