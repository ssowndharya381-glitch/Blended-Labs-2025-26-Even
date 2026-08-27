# Lab 3 – Introduction to Amazon Elastic Compute Cloud (EC2)

## Author

* **Name**: SOWNDHARYA S
* **Register Number**: 212225220100
* **Date of Submission**: 27-08-2026

## Objective

The objective of this experiment is to understand the fundamentals of Amazon Elastic Compute Cloud (EC2). This lab focuses on launching and managing a virtual server, understanding instance types and AMIs, connecting to an EC2 instance, monitoring its status, and performing basic instance operations such as start, stop, and terminate.


## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* Web browser with internet connectivity
* Basic knowledge of Linux commands (optional)

## Tools Used

* AWS Management Console
* Amazon EC2
* Key Pair
* Security Group
* SSH Client (PuTTY / Terminal)

## Tasks Performed

### Task 1: Explore Amazon EC2 Dashboard

Explore the EC2 service dashboard in the AWS Management Console. Observe the different sections such as Instances, AMIs, Instance Types, Key Pairs, Security Groups, and Elastic IPs.

### Task 2: Launch an EC2 Instance

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type (t2.micro) under the free tier. Configure basic settings such as instance name, key pair, and security group.

### Task 3: Configure Security Group

Configure a security group to allow inbound access:

* SSH (Port 22) from your IP address
* HTTP (Port 80) from anywhere (0.0.0.0/0)

This security group acts as a firewall for the instance.

### Task 4: Connect to EC2 Instance

Connect to the running EC2 instance using SSH. Use the downloaded key pair and connect via terminal or PuTTY.

For Amazon Linux:
ssh -i "keyname.pem" ec2-user@<Public-IP>

### Task 5: Perform Basic Instance Operations

Perform the following operations from the EC2 console:

* Stop the instance
* Start the instance
* Reboot the instance

Observe the state changes of the instance.

### Task 6: Monitor EC2 Instance

Monitor the EC2 instance using the Monitoring tab. Observe metrics such as CPU utilization, network in/out, and instance status checks.
### Task 7: Terminate EC2 Instance

Terminate the EC2 instance after completing the experiment to avoid unnecessary AWS charges.

## Workflow (Student Explanation)
Open the AWS Management Console and navigate to the Amazon EC2 service.
Explore the EC2 dashboard and check Instances, AMIs, Instance Types, Key Pairs, and Security Groups.
Launch a new EC2 instance using the Amazon Linux 2 AMI and select the t2.micro instance type.
Provide an instance name, select/create a Key Pair, and configure a Security Group.
Allow SSH (Port 22) access from the required IP address and HTTP (Port 80) access from anywhere.
Launch the instance and wait until the Instance State becomes Running and the status checks are completed.
Connect to the running instance using SSH with the downloaded .pem key file and the instance's Public IP address.

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Dashboard / Instance List
<img width="749" height="329" alt="Screenshot 2026-08-27 093701" src="https://github.com/user-attachments/assets/c9fc3305-e475-45cf-8e45-c4bf987f21e4" />

### Screenshot 2: SSH Connection to Instance
<img width="952" height="437" alt="Screenshot 2026-08-22 220301" src="https://github.com/user-attachments/assets/ac4fa9f4-22f9-4d2f-972e-6061ae90a6d9" />

### Screenshot 3: Instance Monitoring / Status
<img width="745" height="337" alt="Screenshot 2026-08-27 093645" src="https://github.com/user-attachments/assets/5bac3c6b-4cd6-42dc-961c-e0329603ad6d" />


## Result 

This experiment provided hands-on experience with Amazon EC2 by demonstrating how to launch, connect, manage, and monitor a virtual server in AWS. It helped in understanding the concept of Infrastructure as a Service (IaaS) and how compute resources can be provisioned and controlled on demand in the cloud.
