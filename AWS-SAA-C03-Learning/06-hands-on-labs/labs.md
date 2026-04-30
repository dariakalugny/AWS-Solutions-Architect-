# Hands-On Labs

These labs are designed to reinforce exam concepts. Keep screenshots, commands, and notes as evidence of practice.

## Lab 1: Secure VPC Baseline

Build:

- 1 VPC
- 2 public subnets
- 2 private subnets
- Internet gateway
- NAT gateway
- Route tables
- Security groups

Practice:

- Explain which resources are public and private.
- Explain why private instances do not need public IPs.
- Compare Security Groups and NACLs.

## Lab 2: Highly Available Web App

Build or diagram:

- ALB across two Availability Zones
- Auto Scaling Group
- EC2 instances in private subnets
- CloudWatch alarm

Practice:

- Explain how the system survives instance failure.
- Explain how health checks work.
- Explain scaling policies.

## Lab 3: S3 Secure Static Website Pattern

Build or diagram:

- S3 bucket
- CloudFront distribution
- ACM certificate
- Route 53 DNS record
- Bucket policy restricted to CloudFront

Practice:

- Explain why CloudFront is better than exposing S3 directly.
- Explain caching behavior.
- Explain encryption in transit.

## Lab 4: Serverless API Pattern

Build or diagram:

- API Gateway
- Lambda
- DynamoDB
- CloudWatch Logs
- IAM execution role

Practice:

- Explain why this is highly available by default.
- Explain Lambda permissions.
- Explain DynamoDB partition key design basics.

## Lab 5: Decoupled Order Processing

Build or diagram:

- API Gateway or ALB
- Lambda or EC2 producer
- SQS queue
- Worker Lambda or EC2 Auto Scaling workers
- DLQ

Practice:

- Explain retry behavior.
- Explain why SQS improves resilience.
- Explain when to choose FIFO vs Standard queue.

## Lab 6: Disaster Recovery Design

Create diagrams for:

- Backup and restore
- Pilot light
- Warm standby
- Active-active

Practice:

- Compare cost, RTO, and RPO.
- Choose the best strategy for different business requirements.

