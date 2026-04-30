# Simulation Exam 01 - SAA-C03

Answer the questions before opening the answer key. These questions are original practice questions written in the style of the AWS Solutions Architect Associate exam.

## Questions

### Question 1

A company runs a web application on EC2 instances behind an Application Load Balancer. The application must remain available if one Availability Zone fails. What should the solutions architect do?

A. Deploy all EC2 instances in one private subnet and enable detailed monitoring  
B. Deploy EC2 instances across multiple Availability Zones in an Auto Scaling group  
C. Deploy EC2 instances in one Availability Zone and create EBS snapshots every hour  
D. Use one larger EC2 instance type and attach multiple EBS volumes  

### Question 2

A company stores static images and JavaScript files for a global website. Users report high latency from distant locations. Which solution improves performance with the least operational overhead?

A. Store the files on EBS volumes in multiple Regions  
B. Use Amazon S3 with Amazon CloudFront  
C. Use Amazon EFS with mount targets in multiple Availability Zones  
D. Use AWS Storage Gateway  

### Question 3

An application needs a relational database that can automatically fail over during an Availability Zone outage. The application does not require additional read scaling. What should be used?

A. Amazon RDS Multi-AZ  
B. Amazon RDS Read Replica  
C. Amazon DynamoDB Global Tables  
D. Amazon ElastiCache  

### Question 4

A workload processes video files. Jobs can be interrupted and restarted. The company wants to minimize compute cost. What should be used?

A. EC2 On-Demand Instances  
B. EC2 Reserved Instances  
C. EC2 Spot Instances  
D. Dedicated Hosts  

### Question 5

A company needs to decouple an order service from a payment processing service. Orders must be stored until the payment service can process them. What should be used?

A. Amazon SQS  
B. Amazon CloudFront  
C. AWS CloudTrail  
D. AWS Config  

### Question 6

A Lambda function needs permission to read items from a DynamoDB table. What is the best security practice?

A. Store AWS access keys in Lambda environment variables  
B. Attach an IAM role with least-privilege permissions to the Lambda function  
C. Use the AWS root account credentials  
D. Make the DynamoDB table public  

### Question 7

A company needs to audit all API calls made in its AWS account. Which service should be used?

A. Amazon CloudWatch Metrics  
B. AWS CloudTrail  
C. Amazon Inspector  
D. AWS WAF  

### Question 8

A private EC2 instance needs to download software updates from the internet, but it must not have a public IP address. What should be configured?

A. Internet Gateway attached directly to the private subnet  
B. NAT Gateway in a public subnet with route table updates  
C. VPC peering connection  
D. AWS Direct Connect  

### Question 9

A company needs DNS routing that sends users to the Region with the lowest latency. Which Route 53 routing policy should be used?

A. Weighted routing  
B. Latency-based routing  
C. Failover routing  
D. Simple routing  

### Question 10

A company stores rarely accessed archive data and wants the lowest storage cost. Retrieval can take several hours. Which storage class should be used?

A. S3 Standard  
B. S3 Standard-IA  
C. S3 Glacier Deep Archive  
D. EBS Cold HDD  

### Question 11

A web application receives repeated read requests for the same database records. The database is under heavy read load. What can reduce latency and database load?

A. Amazon ElastiCache  
B. AWS CloudFormation  
C. AWS Shield  
D. Amazon Macie  

### Question 12

A company needs to protect an application from common web attacks such as SQL injection and cross-site scripting. What should be used?

A. AWS WAF  
B. Amazon GuardDuty  
C. AWS KMS  
D. Amazon CloudWatch Logs  

### Question 13

A company has many VPCs that need centralized routing to an on-premises network. VPC peering is becoming difficult to manage. What should be used?

A. NAT Gateway  
B. Transit Gateway  
C. Internet Gateway  
D. Egress-only Internet Gateway  

### Question 14

A company needs serverless orchestration for a workflow with multiple Lambda functions and retries. What should be used?

A. AWS Step Functions  
B. Amazon S3  
C. Amazon EBS  
D. AWS Trusted Advisor  

### Question 15

An application needs a NoSQL database with single-digit millisecond performance at large scale. What should be used?

A. Amazon DynamoDB  
B. Amazon RDS for MySQL  
C. Amazon Redshift  
D. Amazon EFS  

### Question 16

A company needs a dedicated private network connection from its data center to AWS with consistent bandwidth. What should be used?

A. AWS Direct Connect  
B. AWS Client VPN  
C. NAT Gateway  
D. Internet Gateway  

### Question 17

A company wants to automatically move S3 objects to cheaper storage as they age. What should be configured?

A. S3 Lifecycle policy  
B. S3 bucket ACL only  
C. EBS snapshot policy  
D. CloudFront cache behavior  

### Question 18

A company needs to store and automatically rotate database credentials. What should be used?

A. AWS Secrets Manager  
B. AWS Certificate Manager  
C. AWS Shield  
D. Amazon Route 53  

### Question 19

A company needs a shared Linux file system mounted by multiple EC2 instances across Availability Zones. What should be used?

A. Amazon EFS  
B. Amazon EBS  
C. Amazon S3 Glacier  
D. Instance store  

### Question 20

A company needs to monitor metrics and create alarms when CPU utilization is high. What should be used?

A. AWS CloudTrail  
B. Amazon CloudWatch  
C. AWS Organizations  
D. Amazon Cognito  

## Answer Key

| Question | Answer | Explanation |
| --- | --- | --- |
| 1 | B | Multi-AZ Auto Scaling behind a load balancer provides high availability. |
| 2 | B | S3 stores static files and CloudFront caches them globally. |
| 3 | A | RDS Multi-AZ provides high availability and automatic failover. |
| 4 | C | Spot Instances are cost-effective for interruptible workloads. |
| 5 | A | SQS provides durable asynchronous decoupling. |
| 6 | B | Lambda should use an IAM execution role with least privilege. |
| 7 | B | CloudTrail records AWS API activity. |
| 8 | B | NAT Gateway allows outbound internet access from private subnets. |
| 9 | B | Latency-based routing sends users to the lowest-latency Region. |
| 10 | C | Glacier Deep Archive is the lowest-cost archive class for long retrieval times. |
| 11 | A | ElastiCache reduces repeated database reads and improves latency. |
| 12 | A | WAF protects against common web attacks. |
| 13 | B | Transit Gateway centralizes routing across many VPCs and networks. |
| 14 | A | Step Functions orchestrates serverless workflows with retries and state. |
| 15 | A | DynamoDB is managed NoSQL with low-latency scale. |
| 16 | A | Direct Connect provides dedicated private connectivity. |
| 17 | A | S3 Lifecycle policies transition objects between storage classes. |
| 18 | A | Secrets Manager stores and rotates secrets. |
| 19 | A | EFS is shared managed NFS storage for Linux workloads. |
| 20 | B | CloudWatch provides metrics and alarms. |

