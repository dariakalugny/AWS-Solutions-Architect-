# Domain 1: Design Secure Architectures

Weight: **30%**

This is the biggest exam domain. Prioritize IAM, VPC security, encryption, secrets, and secure access patterns.

## Must-Know Topics

- IAM users, groups, roles, policies
- Least privilege
- MFA and root account protection
- STS and temporary credentials
- Cross-account access
- AWS Organizations and SCPs
- IAM Identity Center
- Resource policies
- VPC security: Security Groups, NACLs, route tables, NAT gateways
- Public vs private subnets
- KMS, ACM, TLS, encryption at rest and in transit
- Secrets Manager
- WAF, Shield, GuardDuty, Inspector, Macie, Security Hub
- VPN and Direct Connect security considerations

## Exam Thinking

- If an AWS service needs permissions, prefer an IAM role.
- If users need temporary AWS access, think federation or IAM Identity Center.
- If encryption at rest is required, think KMS.
- If HTTPS certificates are required, think ACM.
- If credentials must be rotated, think Secrets Manager.
- If protecting web apps from common attacks, think WAF.
- If DDoS protection is needed, think Shield.
- If threat detection is needed, think GuardDuty.

## Services To Review

- IAM
- IAM Identity Center
- STS
- Organizations
- Control Tower
- KMS
- ACM
- Secrets Manager
- Cognito
- WAF
- Shield
- GuardDuty
- Inspector
- Macie
- Security Hub
- Network Firewall
- CloudHSM
- VPC
- Site-to-Site VPN
- Direct Connect

