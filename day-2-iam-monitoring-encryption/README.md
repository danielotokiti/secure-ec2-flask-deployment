# Day 2 – IAM + Monitoring + Encryption Lab

## Tasks Completed:
- Created IAM Role with S3 Read-Only Access
- Attached IAM Role to EC2 instance
- Verified IAM Role permissions via `aws s3 ls` on EC2
- Created and attached encrypted EBS volume to EC2
- Installed and configured CloudWatch Agent for CPU and memory metrics
- Verified CloudWatch metrics in AWS Console
- Created CloudWatch alarm for CPU utilization > 80%

## Screenshots:
- IAM Role summary page
- EC2 instance details with attached IAM Role
- Terminal output showing `aws s3 ls`
- Encrypted EBS volume details and `lsblk` output
- CloudWatch Agent installation and status
- CloudWatch metrics dashboard
- CloudWatch alarm configuration summary

## Notes:
- IAM roles enable secure access without hardcoding credentials
- Encrypted EBS volumes protect data at rest
- CloudWatch monitoring is essential for proactive infrastructure health
