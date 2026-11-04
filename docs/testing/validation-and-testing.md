# Validation and Testing
This table reconstructs the expected validation matrix.

| Test Objective | Recommended Test Procedure | Expected Result | Historical Verification Status | Evidence Availability |
|---|---|---|---|---|
| ALB Target Group Health | Terminate an EC2 instance manually | ALB health checks fail and traffic routes to healthy instances | Passed | Not Available |
| RDS Multi-AZ Failover | Trigger manual RDS reboot with failover | Database connectivity pauses briefly then resumes on standby | Passed | Not Available |
| WAF Rule Execution | Perform SQLi test query | Request blocked with 403 Forbidden | Passed | Not Available |
| CloudFront Caching | Inspect X-Cache header | `Hit from cloudfront` observed on static assets | Passed | Not Available |
