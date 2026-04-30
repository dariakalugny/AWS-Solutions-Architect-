# Domain 4: Design Cost-Optimized Architectures

Weight: **20%**

This domain tests whether you can meet requirements at the lowest reasonable cost.

## Must-Know Topics

- EC2 purchasing options
- Savings Plans
- Reserved Instances
- Spot Instances
- Storage classes
- Lifecycle policies
- Data transfer costs
- NAT Gateway costs
- Right sizing
- Auto Scaling
- Serverless cost models
- Database capacity modes
- Cost monitoring tools

## Cost Tools

- AWS Cost Explorer
- AWS Budgets
- Cost and Usage Report
- Trusted Advisor
- Compute Optimizer
- Cost allocation tags

## Storage Cost Thinking

- S3 Standard: frequently accessed data
- S3 Intelligent-Tiering: unknown or changing access patterns
- S3 Standard-IA: infrequent access, rapid retrieval
- S3 One Zone-IA: infrequent access, lower resilience
- S3 Glacier: archive
- S3 Glacier Deep Archive: lowest-cost archive

## Compute Cost Thinking

- On-Demand: flexible, no commitment
- Reserved Instances: predictable steady usage
- Savings Plans: flexible committed spend
- Spot Instances: fault-tolerant interruptible workloads
- Lambda/Fargate: reduce operational overhead and pay by usage pattern

## Exam Thinking

- If workload is interruptible, consider Spot.
- If workload is steady, consider Savings Plans or Reserved Instances.
- If access pattern is unknown, consider S3 Intelligent-Tiering.
- If data is archival, consider S3 Glacier classes.
- If NAT Gateway cost is high, consider VPC endpoints for AWS services.
- If database demand is unpredictable, consider serverless or on-demand capacity.

