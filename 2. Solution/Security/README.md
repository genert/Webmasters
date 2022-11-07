
---

# Security

There are many aspect of security to consider, including Authentication and Authorisation.

The following is an overview of the security considerations for the Hey Blue solution, which will be deployed using AWS.


## Identity & Access Management (Authentication & Authorisation)

AWS Identity Services can be used to manage resources, identities and access, at scale if required.

Service options:

- IAM (AWS Identity Access Management) - most likely for development, deployment, and similar
- SSO (Single Sign On) - for development, deployment, and similar
- Amazon Cognito - identity management for users of Hey Blue

## Data Law & Compliance

Compliance status and monitoring are part of AWS services, therefore Hey Blue can choose which standards and best practices to adhere to and have these automatically monitored.

Service options:

- AWS Audit Manager - audit AWS usage for risk assessment and compliance
- AWS Artifact - compliance reporting

## Network & Infrastructure

Fine-grained security policies can be enforced on network traffic, particularly important when interfacing with other systems. We can use these controls to create a Zero Trust infrastructure to help protect against intruders who may manage to circumnavigate authentication controls.

Service options:

- AWS Shield - DDoS protection
- AWS WAF (Web Application Firewall), AWS Network Firewall, & AWS Firewall Manager - filter malicious traffic and implement zero-trust

## Data Protection

AWS includes services such as Encryption and Key Management, allowing services to have their own authentication and authorisation, rather than storing secrets in code.

Data will be encrypted when at rest (e.g. in a database) and in transit, with appropriately strong encryption.

Passwords will be stored only as salted hashes and the policy for length and complexity will follow current best practice (e.g. 10+ characters, at least 256 character higher length limit, NO need to include specific character types, check hacked/common password lists, NO need to change every x months, etc), and best practice password tips will be displayed.

Service options:

- KMS (Key Management Service) - encryption key storage and management
- AWS Certificate Manager - manage public and private SSL/TLS certificates
- AWS Secrets Manager - manage, rotate and retrieve secrets

## Threat Detection & Monitoring

AWS provides services to continuously monitor network activity and behaviour of accounts/users, in order to identify threats at the earliest opportunity.

Service options:

- AWS Security Hub - monitor compliance and security
- Amazon GuardDuty - threat detection
- AWS CloudTrail - log and track activity
- Amazon Detective - investigate potential threats and issues
- CloudEndure Disaster Recovery - recover from outages or malicious attacks
