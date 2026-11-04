# Network Design
## Amazon VPC and Networking
**Reconstructed Architecture**: The VPC spans two Availability Zones to maintain fault tolerance.
- **Public Subnets**: Route outbound traffic directly to the Internet Gateway. Hosts NAT Gateways and ALB.
- **Private Application Subnets**: No direct internet route. Outbound traffic routes to NAT Gateways.
- **Private Database Subnets**: Completely isolated.
- **Network ACLs**: Stateless return traffic considered, especially for ephemeral ports.
- **Security Groups**: Stateful protection. EC2 only allows inbound from ALB. RDS only allows inbound from EC2 SG.
