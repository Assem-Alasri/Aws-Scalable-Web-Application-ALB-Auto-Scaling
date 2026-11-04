# Security Architecture
## Framework Review: Security Pillar
- **Identity and Access Management**: SSM requires EC2 instances to have the `AmazonSSMManagedInstanceCore` managed policy.
- **Detective Controls**: Amazon CloudWatch for metrics and AWS WAF logs for web traffic monitoring.
- **Infrastructure Protection**: VPC boundaries, Subnet tiering, Security Groups acting as stateful firewalls.
- **Data Protection**: Encryption in transit via HTTPS/TLS handled by ALB. 
**Reconstructed Architecture Note**: The exact historical configuration of IAM roles and WAF rules (e.g., AWSManagedRulesCommonRuleSet) is considered recommended baseline, as exact historical IDs are unavailable.
