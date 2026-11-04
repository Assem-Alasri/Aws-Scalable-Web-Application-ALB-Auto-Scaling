# Auto Scaling and High Availability
## Framework Review: Reliability & Performance Efficiency
- **EC2 Auto Scaling**: Deploys instances uniformly across AZ A and AZ B. 
- **Target Tracking Scaling**: Automatically adjusts desired capacity based on CPU Utilization or ALB Request Count.
- **Application Load Balancer**: Distributes incoming dynamic requests. Health checks configured to rapidly deregister unresponsive targets.
- **NAT Gateway Availability**: Proposed reference design allocates one NAT Gateway per AZ to avoid a single point of failure.
