# Starter Practice Questions

For longer exam-style practice, use:

- [Simulation Exam 01](simulation-exam-01.md)
- [Simulation Exam 02](simulation-exam-02.md)
- [Simulation Score Tracker](simulation-score-tracker.md)

## Question 1

A company needs a relational database to remain available during an Availability Zone failure. The application does not need extra read capacity. What should you choose?

Answer:

RDS Multi-AZ.

Why:

Multi-AZ provides high availability and automatic failover. Read replicas are for read scaling, not primarily for HA.

## Question 2

A workload processes image files. Processing can be interrupted and restarted. The company wants the lowest EC2 cost. What should you choose?

Answer:

Spot Instances.

Why:

Spot is best for fault-tolerant, interruptible workloads.

## Question 3

A static website has global users and must have low latency. What should you choose?

Answer:

Amazon S3 with Amazon CloudFront.

Why:

S3 stores the static content. CloudFront caches content at edge locations near users.

## Question 4

An application has traffic spikes and uses a relational database. Repeated reads are causing database load. What can improve read latency?

Answer:

Amazon ElastiCache.

Why:

ElastiCache stores frequently accessed data in memory and reduces database load.

## Question 5

A company needs to decouple an application producer from consumers and ensure messages are processed asynchronously. What should you choose?

Answer:

Amazon SQS.

Why:

SQS is a queue service used for decoupling and asynchronous processing.

## Question 6

A company needs to audit API calls made in an AWS account. What service should be enabled?

Answer:

AWS CloudTrail.

Why:

CloudTrail records AWS API activity for auditing and investigation.

## Question 7

A workload needs DNS failover between healthy and unhealthy endpoints. What service and feature should you use?

Answer:

Amazon Route 53 failover routing with health checks.

Why:

Route 53 can monitor endpoint health and route traffic to a healthy endpoint.

## Question 8

A company has unknown S3 access patterns and wants automatic cost optimization without operational work. What storage class should be used?

Answer:

S3 Intelligent-Tiering.

Why:

It automatically moves objects between access tiers based on changing access patterns.
