---
layout: default
title: IAM Users
type: page
---

## AWS Identities
  - IAM User
    - A person
    - A service
  - IAM Group
  - IAM Role

## IAM Users
  - Receives unique name and unique identifier ARN (Amazon Resource Name)
  - Access securely through unique credentials
  - Access appropraite resources through assigned permissions

## Access Types
  - AWS Management Console - requires account id (or alias), username and password.
  - Programmatic - Requires access keys (Key ID and Secret Access Key) - useful for AWS CLI, SDKs, Rest or Query operations.

## Access Keys Best Practice
  - Delete access keys for root
  - Assign to appropriate users
  - Securely store saccess key
  - Rotate at least every 90 days
  - Monitor and deactivate
  - Delete unused

## Mutlti-Factor Authentication (MFA)
  - Allows you to apply 2 levels of authentication
  - Creates a random 6 digit single use authentication code
  - Code changes every 30 seconds

### MFA Types
  - Virtual MFA device - Google Authenticator, Windows Authenticator, Authy
  - Hardware
  - Universal 2nd FActor (U2F) security key

### MFA Best Practice
  - Enable for root
  - Enable for privileged IAM users

## AWS Root User
- All AWS accounts have root user
- Unrestricted access to all AWS services and resources

**You should not access root on daily basis**

Use root account for the following:
  - Change AWS support plan
  - Change payment options
  - View billing
  - Close account

### Best Practices
  - Activate MFA
  - Disable root keys
  - Rotate credentials
  - Do not share credentials
  - **Create IAM user with administrative privileges**





