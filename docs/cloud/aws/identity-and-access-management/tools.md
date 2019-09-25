---
layout: default
title: Tools
type: page
---
# IAM Access Control Tools
- Credential Report: Identity based reports in CSV format. HJelp improve security and compliance.
- Access Advisor: Used to monitor policies, useful for seeing if users are using assigned resources.
- AWS CloudTrail: see below
- AWS Trusted Advisor: see below
- AWS Config: see below

## AWS CloudTrail
### Activities
- AWS console
- AWS CLI
- AWS SDK
- Other services
  
### Benefits
- Visibility
- Compliance
- Analysis
- Troubleshooting
  
### Events
- Management
- Data
  
### Features
- Record account activity and service events from most AWS services
- Record activity from one or all regions in AWS account
- Record activity from multiple accounts in a common S3 bucket
- Enable log file and file integrity validation
  
### Useful for
- Failed logins
- IAM changes
- Authorization failures
- Resource modification

## Trusted Advisor
Compares AWS accounts against good practice, thus improving security  and performance. Checks include:
- Cost
- Performance
- Security
- Fault tolerance
- Service limits

## AWS Config
Assess, audit and evaluate configuration of AWS resources, benefits include:
- Continuous monitoring and assessment
- Change management
- Operational troubleshooting
- Enterprise compliance
Examples of areas that can be monitored in IAM include:
- MFA
- Password policies
- IAM policy blacklist
- Group checks
- Policies applied direct to users.


