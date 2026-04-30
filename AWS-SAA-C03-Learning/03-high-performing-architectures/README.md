# Domain 3: Design High-Performing Architectures

Weight: **24%**

This domain tests whether you can choose services and configurations that meet performance, scaling, and latency requirements.

## Must-Know Topics

- Object vs block vs file storage
- Compute selection
- Horizontal vs vertical scaling
- Caching
- Database performance and read scaling
- Edge networking
- Data ingestion and streaming
- Analytics processing
- Network performance

## Storage Performance

- S3: object storage, massive scale, static assets, data lakes
- EBS: block storage for EC2, low-latency disks
- EFS: shared file storage, Linux workloads, multi-AZ
- FSx: managed high-performance file systems

## Compute Performance

- EC2: maximum control and instance family selection
- Lambda: event-driven serverless workloads
- Fargate: serverless containers
- ECS/EKS: container orchestration
- Batch: batch processing
- EMR: big data processing

## Database Performance

- RDS read replicas for read scaling
- Aurora for high-performance relational workloads
- DynamoDB for massive scale key-value access
- ElastiCache for low-latency caching
- Redshift for data warehousing
- OpenSearch for search and log analytics

## Exam Thinking

- Use CloudFront for global content delivery.
- Use Global Accelerator for improving global network path to applications.
- Use ElastiCache when repeated database reads cause latency.
- Use DynamoDB for predictable key-value access at scale.
- Use Kinesis for streaming data.
- Use Glue for ETL.
- Use Athena for serverless SQL queries on S3 data.

## Services To Review

- S3
- EBS
- EFS
- FSx
- EC2
- Lambda
- Fargate
- ECS
- EKS
- Batch
- EMR
- RDS
- Aurora
- DynamoDB
- ElastiCache
- Redshift
- CloudFront
- Global Accelerator
- Kinesis
- Glue
- Athena
- QuickSight

