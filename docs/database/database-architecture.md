# Database Architecture
## Amazon RDS Multi-AZ
**User-Reported Implementation**: The system utilized Amazon RDS configured for Multi-AZ.
- **Primary Instance**: Resides in Private DB Subnet A.
- **Standby Instance**: Resides in Private DB Subnet B.
- **Failover**: Automatic DNS propagation seamlessly shifts database endpoints from Primary to Standby during outages.
