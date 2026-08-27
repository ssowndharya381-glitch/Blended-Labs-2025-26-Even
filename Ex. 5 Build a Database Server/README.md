# Lab 5 – Build a Database Server (AWS)

## Author

* **Name**:SOWNDHARYA S
* **Register Number**:212225220100
* **Date of Submission**: 27-08-2026
* 
## Objective

The objective of this experiment is to understand how to deploy and configure a database server in AWS. This lab focuses on launching an EC2 instance, installing a database management system (DBMS), configuring basic database settings, creating a sample database, and validating connectivity to the database server.

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* An existing VPC and EC2 knowledge (from previous labs)
* Basic knowledge of Linux commands and SQL

## Tools Used

* AWS Management Console
* Amazon EC2
* Security Groups
* SSH Client (Terminal / PuTTY)
* MySQL / MariaDB / PostgreSQL (any one)


## Tasks Performed

### Task 1: Launch EC2 Instance for Database Server

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type and configure key pair and security group.


### Task 2: Configure Security Group for Database Access

Modify the security group to allow:

* SSH (Port 22) for remote access
* Database port (e.g., MySQL – 3306 or PostgreSQL – 5432)


### Task 3: Connect to EC2 Instance

Connect to the EC2 instance using SSH from your local machine.


### Task 4: Install Database Server

Install a database server software such as MySQL, MariaDB, or PostgreSQL on the EC2 instance using package manager commands.

### Task 5: Start and Configure Database Service

Start the database service and configure basic settings such as root password and user privileges.

### Task 6: Create a Sample Database

Create a sample database and a table inside it. Insert a few records into the table.


### Task 7: Test Database Connectivity

Test the database server by connecting to it locally or remotely and performing basic SQL queries.

### Workflow (Student Explanation)
Open the AWS Management Console and navigate to the Amazon EC2 service.  
Explore the EC2 dashboard and check Instances, AMIs, Instance Types, Key Pairs, and Security Groups.  
Launch a new EC2 instance using the Amazon Linux 2 AMI and select the t2.micro instance type.  
Provide an instance name, select/create a Key Pair, and configure a Security Group.  
Allow SSH (Port 22) access from the required IP address and HTTP (Port 80) access from anywhere.  
Launch the instance and wait until the Instance State becomes Running and the status checks are completed.    
Connect to the running instance using SSH with the downloaded .pem key file and the instance's Public IP address.  

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Instance for Database Server
<img width="596" height="287" alt="image" src="https://github.com/user-attachments/assets/a8961b87-47b7-4395-b7cb-b8c1a24b3bb6" />

### Screenshot 2: Database Service Running
<img width="636" height="315" alt="image" src="https://github.com/user-attachments/assets/2d2b7e34-1773-4651-872e-75597fbadac7" />

### Screenshot 3: Sample Database and Table

## Result

This experiment demonstrated how to build a database server in AWS using an EC2 instance. By installing and configuring a DBMS, creating a sample database, and testing connectivity, the fundamentals of hosting and managing a cloud-based database server were underst
