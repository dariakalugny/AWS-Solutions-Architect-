# Domain 2: Design Resilient Architectures

Weight: **26%**

This domain focuses on high availability, fault tolerance, loose coupling, disaster recovery, and reducing single points of failure.

## Must-Know Topics

- Multi-AZ design
- Multi-Region design
- Load balancing
- Auto Scaling
- Stateless vs stateful workloads
- Queues and pub/sub
- Event-driven architecture
- Serverless design
- Read replicas
- Backups and replication
- Disaster recovery strategies
- RTO and RPO
- Service quotas and throttling

## Disaster Recovery Strategies

| Strategy | Cost | Recovery Speed | Notes |
| --- | --- | --- | --- |
| Backup and restore | Lowest | Slowest | Good for low-cost DR |
| Pilot light | Low | Medium | Core services always running |
| Warm standby | Medium | Faster | Scaled-down full environment |
| Active-active | Highest | Fastest | Multiple live Regions |

## Exam Thinking

- Multi-AZ is the default answer for high availability inside one Region.
- Multi-Region is for disaster recovery, global latency, or regional failure requirements.
- SQS helps decouple components.
- SNS helps fan out messages.
- EventBridge routes events across services and systems.
- Step Functions orchestrates workflows.
- RDS Multi-AZ improves availability, not read performance.
- RDS read replicas improve read scalability.

## Services To Review

- ELB
- EC2 Auto Scaling
- AWS Auto Scaling
- SQS
- SNS
- EventBridge
- Step Functions
- Lambda
- API Gateway
- ECS
- EKS
- Fargate
- RDS
- Aurora
- DynamoDB Global Tables
- S3 replication
- Route 53 failover routing
- CloudWatch
- X-Ray

