# Service Decision Guide

Use this file when two services look similar in an exam question.

## S3 vs EBS vs EFS vs FSx

| Need | Choose |
| --- | --- |
| Object storage, static files, backups, data lake | S3 |
| Block storage attached to EC2 | EBS |
| Shared Linux file system | EFS |
| Managed Windows, Lustre, NetApp, OpenZFS file systems | FSx |

## RDS Multi-AZ vs Read Replica

| Need | Choose |
| --- | --- |
| High availability and failover | RDS Multi-AZ |
| Scale read traffic | Read Replica |
| Cross-Region read or DR support | Cross-Region Read Replica |

## ALB vs NLB vs Gateway Load Balancer

| Need | Choose |
| --- | --- |
| HTTP/HTTPS, host/path routing | ALB |
| TCP/UDP/TLS, very high performance, static IP support | NLB |
| Third-party security appliances or packet inspection | Gateway Load Balancer |

## SQS vs SNS vs EventBridge

| Need | Choose |
| --- | --- |
| Queue and decouple producer from consumer | SQS |
| Fanout notifications to many subscribers | SNS |
| Event routing between AWS services, SaaS, and apps | EventBridge |

## Lambda vs ECS/Fargate vs EC2

| Need | Choose |
| --- | --- |
| Short event-driven function, no server management | Lambda |
| Containers without managing servers | ECS with Fargate |
| Kubernetes orchestration | EKS |
| Full OS control or legacy workload | EC2 |

## CloudFront vs Global Accelerator

| Need | Choose |
| --- | --- |
| Cache static or dynamic content at edge locations | CloudFront |
| Improve global network path for TCP/UDP applications | Global Accelerator |

## VPN vs Direct Connect

| Need | Choose |
| --- | --- |
| Fast setup, encrypted connection over internet | Site-to-Site VPN |
| Dedicated private connectivity and consistent bandwidth | Direct Connect |
| User VPN access to AWS | Client VPN |

## NAT Gateway vs VPC Endpoint

| Need | Choose |
| --- | --- |
| Private subnet resources need outbound internet access | NAT Gateway |
| Private access to AWS services without internet path | VPC Endpoint |
| Reduce NAT data processing cost for AWS service traffic | VPC Endpoint |

## KMS vs Secrets Manager vs ACM

| Need | Choose |
| --- | --- |
| Encryption key management | KMS |
| Store and rotate credentials/secrets | Secrets Manager |
| TLS/SSL certificates | ACM |

## CloudWatch vs CloudTrail vs Config

| Need | Choose |
| --- | --- |
| Metrics, logs, alarms, dashboards | CloudWatch |
| Audit API calls and account activity | CloudTrail |
| Track resource configuration and compliance | AWS Config |

## GuardDuty vs Inspector vs Macie

| Need | Choose |
| --- | --- |
| Threat detection from logs and signals | GuardDuty |
| Vulnerability management for workloads | Inspector |
| Sensitive data discovery in S3 | Macie |

## Route 53 Routing Policies

| Need | Choose |
| --- | --- |
| One record, basic DNS response | Simple |
| Split traffic by percentage | Weighted |
| Route to lowest-latency Region | Latency-based |
| Active-passive disaster recovery | Failover |
| Route by user location | Geolocation |
| Return multiple healthy records | Multi-value answer |

