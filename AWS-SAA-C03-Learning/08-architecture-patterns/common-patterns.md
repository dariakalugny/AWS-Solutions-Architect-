# Common Architecture Patterns

## Three-Tier Web Application

```mermaid
flowchart TD
    Users[Users] --> R53[Route 53]
    R53 --> CF[CloudFront]
    CF --> ALB[Application Load Balancer]
    ALB --> ASG[Auto Scaling Group - Web/App Tier]
    ASG --> RDS[(RDS Multi-AZ)]
    ASG --> S3[(S3 Static Assets)]
    ASG --> CW[CloudWatch]
```

Use when:

- You need a classic scalable web app.
- You need managed relational database storage.
- You need high availability across Availability Zones.

## Serverless API

```mermaid
flowchart TD
    Client[Client] --> APIGW[API Gateway]
    APIGW --> Lambda[Lambda]
    Lambda --> DDB[(DynamoDB)]
    Lambda --> CW[CloudWatch Logs]
```

Use when:

- You want low operational overhead.
- Traffic is variable.
- Event-driven execution fits the workload.

## Decoupled Processing

```mermaid
flowchart LR
    Producer[Producer] --> Queue[SQS Queue]
    Queue --> Worker[Worker Fleet or Lambda]
    Worker --> DB[(Database)]
    Queue --> DLQ[Dead-Letter Queue]
```

Use when:

- Producers and consumers scale differently.
- You need buffering.
- Failures should not immediately break the whole workflow.

## Global Static Content

```mermaid
flowchart TD
    Users[Global Users] --> R53[Route 53]
    R53 --> CF[CloudFront]
    CF --> S3[(S3 Origin)]
    CF --> WAF[AWS WAF]
```

Use when:

- Content is static or cacheable.
- Users are geographically distributed.
- You need lower latency and edge caching.

## Hybrid Connectivity

```mermaid
flowchart LR
    OnPrem[On-Premises Data Center] --> DX[Direct Connect]
    OnPrem --> VPN[Site-to-Site VPN]
    DX --> TGW[Transit Gateway]
    VPN --> TGW
    TGW --> VPC1[VPC A]
    TGW --> VPC2[VPC B]
```

Use when:

- A company needs private connectivity to AWS.
- Multiple VPCs need centralized routing.
- VPN can be backup for Direct Connect.
