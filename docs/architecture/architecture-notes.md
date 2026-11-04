# Architecture Notes
This directory contains the reconstructed solution architecture diagram for the Scalable Web Application project.

## Reconstructed Architecture
As the original deployment was deleted and configuration state files are unavailable, this diagram serves as a reconstructed reference architecture based on reported design goals and AWS best practices.

## Assumptions
- **AWS WAF**: Assumed as a Regional Web ACL attached to the Application Load Balancer. CloudFront may also have an edge-optimized WAF, but this reference design explicitly models the ALB association.
- **NAT Gateways**: One NAT Gateway per Availability Zone is recommended and modeled for true high availability.
