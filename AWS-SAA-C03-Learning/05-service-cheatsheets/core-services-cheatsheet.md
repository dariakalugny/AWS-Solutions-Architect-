# Core Services Cheatsheet

## IAM

- Controls identity and access.
- Use roles for AWS services and temporary credentials.
- Apply least privilege.
- Root user should have MFA and should not be used for daily tasks.

## VPC

- Your private network in AWS.
- Public subnet has a route to an internet gateway.
- Private subnet usually reaches the internet through a NAT gateway.
- Security Groups are stateful; Network ACLs are stateless.

## EC2

- Virtual servers.
- Best when you need OS-level control.
- Use Auto Scaling Groups for elasticity and availability.
- Use Spot for interruptible workloads, Reserved Instances or Savings Plans for predictable usage.

## ELB

- Application Load Balancer: HTTP/HTTPS, layer 7, path and host routing.
- Network Load Balancer: TCP/UDP/TLS, layer 4, very high performance.
- Gateway Load Balancer: third-party appliances and network inspection.

## S3

- Object storage.
- Highly durable.
- Supports versioning, lifecycle policies, replication, encryption, event notifications.
- Not a file system and not block storage.

## EBS

- Block storage for EC2.
- Tied to an Availability Zone.
- Snapshots are stored in S3.
- Use Provisioned IOPS for high-performance transactional workloads.

## EFS

- Managed NFS file system.
- Multi-AZ access.
- Good for shared Linux file storage.

## RDS

- Managed relational database.
- Multi-AZ is for high availability.
- Read replicas are for read scaling.
- Automated backups support point-in-time recovery.

## Aurora

- AWS-optimized relational database compatible with MySQL and PostgreSQL.
- High performance and high availability.
- Aurora Global Database is useful for global reads and DR.

## DynamoDB

- Managed NoSQL key-value and document database.
- Single-digit millisecond performance.
- Global Tables support multi-Region active-active patterns.
- Use DAX for read-heavy caching.

## Lambda

- Serverless compute.
- Best for event-driven workloads.
- Pay per invocation and duration.
- Watch timeout, package size, cold starts, and VPC networking considerations.

## SQS

- Queue service for decoupling.
- Standard queue: high throughput, at-least-once delivery, best-effort ordering.
- FIFO queue: ordering and exactly-once processing within limits.

## SNS

- Pub/sub messaging.
- Fanout to SQS, Lambda, HTTP endpoints, email, SMS.

## EventBridge

- Event bus for event-driven architectures.
- Best for routing events between AWS services, SaaS, and custom applications.

## Route 53

- DNS service.
- Routing policies include simple, weighted, latency, failover, geolocation, and multi-value answer.

## CloudFront

- CDN for caching content at edge locations.
- Improves latency and can reduce origin load.
- Often paired with S3, ALB, API Gateway.

## CloudWatch

- Metrics, logs, alarms, dashboards.
- Used for monitoring and operational visibility.

## CloudTrail

- Records API activity.
- Important for auditing and security investigations.

## KMS

- Managed encryption keys.
- Used by many AWS services for encryption at rest.
- Know AWS managed keys vs customer managed keys.

