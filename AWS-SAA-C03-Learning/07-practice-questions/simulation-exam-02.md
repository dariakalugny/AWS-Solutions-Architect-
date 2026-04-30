# Simulation Exam 02 - SAA-C03

This simulation focuses on scenario-based service selection, cost optimization, security, and resilience.

## Questions

### Question 1

A company hosts an application in private subnets. The application must access Amazon S3 without sending traffic through the public internet or NAT Gateway. What should be used?

A. VPC Gateway Endpoint for S3  
B. Internet Gateway  
C. NAT Instance  
D. AWS Client VPN  

### Question 2

A company has an application that requires host-based routing and path-based routing for HTTP requests. Which load balancer should be used?

A. Network Load Balancer  
B. Application Load Balancer  
C. Gateway Load Balancer  
D. Classic Load Balancer  

### Question 3

A company needs to run containers without managing EC2 instances. Which service should be used?

A. Amazon ECS with Fargate  
B. Amazon EC2 Auto Scaling only  
C. Amazon EBS  
D. Amazon Route 53  

### Question 4

A workload has unpredictable traffic and uses DynamoDB. The company does not want to manage capacity. Which capacity mode should be used?

A. Provisioned capacity with no auto scaling  
B. On-demand capacity  
C. Reserved capacity only  
D. Manual sharding  

### Question 5

A company needs active-active NoSQL writes in multiple Regions. Which service feature should be used?

A. RDS Multi-AZ  
B. DynamoDB Global Tables  
C. ElastiCache Redis cluster mode disabled  
D. EBS snapshots copied to another Region  

### Question 6

A company wants to detect suspicious account activity and potential threats using AWS log sources. What should be used?

A. Amazon GuardDuty  
B. AWS Certificate Manager  
C. AWS Budgets  
D. Amazon EFS  

### Question 7

A company needs to analyze data directly in S3 using SQL without managing servers. What should be used?

A. Amazon Athena  
B. Amazon RDS  
C. Amazon EBS  
D. AWS DMS  

### Question 8

A company needs a data warehouse for complex analytical queries over large datasets. What should be used?

A. Amazon Redshift  
B. Amazon ElastiCache  
C. Amazon EFS  
D. AWS CloudTrail  

### Question 9

A company needs to migrate an on-premises database to AWS with minimal downtime. Which service is designed for this?

A. AWS Database Migration Service  
B. AWS Config  
C. Amazon CloudFront  
D. AWS Artifact  

### Question 10

A company needs to send one notification to multiple subscribers including SQS queues and Lambda functions. What should be used?

A. Amazon SNS  
B. Amazon EBS  
C. AWS KMS  
D. Amazon Route 53 Resolver  

### Question 11

A company needs encryption key management for data encrypted by multiple AWS services. What should be used?

A. AWS KMS  
B. AWS Shield Advanced  
C. Amazon Cognito  
D. AWS Trusted Advisor  

### Question 12

A company needs HTTPS certificates for an Application Load Balancer. What should be used?

A. AWS Certificate Manager  
B. AWS Secrets Manager  
C. Amazon Inspector  
D. AWS CloudHSM only  

### Question 13

A company wants to reduce NAT Gateway data processing costs for private subnet access to DynamoDB. What should be used?

A. VPC Endpoint for DynamoDB  
B. More NAT Gateways  
C. Larger EC2 instances  
D. CloudFront signed URLs  

### Question 14

A company needs automatic failover between primary and secondary endpoints based on health checks. Which Route 53 routing policy should be used?

A. Failover routing  
B. Weighted routing  
C. Geoproximity routing only  
D. Simple routing  

### Question 15

A company needs to discover sensitive data such as personally identifiable information in S3 buckets. What should be used?

A. Amazon Macie  
B. AWS WAF  
C. Amazon CloudWatch Metrics  
D. AWS Backup  

### Question 16

A company runs a steady EC2 workload for the next 3 years. It wants to reduce cost while keeping flexibility across instance families. What should be considered?

A. Compute Savings Plans  
B. On-Demand Instances only  
C. Spot Instances only  
D. Dedicated Hosts only  

### Question 17

A company needs a managed message broker compatible with existing RabbitMQ applications. What should be used?

A. Amazon MQ  
B. Amazon SQS only  
C. Amazon SNS only  
D. Amazon EventBridge only  

### Question 18

A company needs to track configuration changes to AWS resources and evaluate compliance rules. What should be used?

A. AWS Config  
B. AWS CloudTrail only  
C. Amazon CloudFront  
D. Amazon ECR  

### Question 19

A company needs centralized control over multiple AWS accounts and wants to apply service control policies. What should be used?

A. AWS Organizations  
B. Amazon Cognito  
C. AWS X-Ray  
D. Amazon Inspector  

### Question 20

A company wants to improve global traffic performance for a TCP application using the AWS global network. What should be used?

A. AWS Global Accelerator  
B. Amazon S3 Transfer Acceleration only  
C. Amazon EFS  
D. AWS Backup  

## Answer Key

| Question | Answer | Explanation |
| --- | --- | --- |
| 1 | A | S3 Gateway Endpoints keep S3 traffic private and avoid NAT Gateway cost. |
| 2 | B | ALB supports layer 7 HTTP/HTTPS routing, including host and path rules. |
| 3 | A | ECS with Fargate runs containers without managing EC2 instances. |
| 4 | B | DynamoDB on-demand is best for unpredictable traffic with no capacity planning. |
| 5 | B | DynamoDB Global Tables provide multi-Region active-active NoSQL replication. |
| 6 | A | GuardDuty detects suspicious activity and threats. |
| 7 | A | Athena runs serverless SQL queries directly against S3 data. |
| 8 | A | Redshift is AWS's managed data warehouse service. |
| 9 | A | DMS supports database migration with minimal downtime. |
| 10 | A | SNS provides pub/sub fanout to multiple subscribers. |
| 11 | A | KMS manages encryption keys for AWS services and applications. |
| 12 | A | ACM provides managed public TLS certificates for ALB and other AWS services. |
| 13 | A | DynamoDB VPC endpoints reduce NAT usage and keep traffic private. |
| 14 | A | Failover routing uses health checks for active-passive DNS failover. |
| 15 | A | Macie discovers sensitive data in S3. |
| 16 | A | Compute Savings Plans fit steady compute usage with flexibility. |
| 17 | A | Amazon MQ supports managed RabbitMQ and ActiveMQ brokers. |
| 18 | A | AWS Config tracks resource configurations and evaluates compliance. |
| 19 | A | Organizations manages multiple accounts and SCPs. |
| 20 | A | Global Accelerator improves global TCP/UDP traffic using AWS edge network. |

