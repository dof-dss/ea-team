---
layout: default
title: Identity and Access Management Best Practices
type: page
---

# IAM Best Practices

## Users

- Lock away root account
- Use individual IAM users
- Do not share credentials
- Rotate credentials
- Remove unnecessary credentials
- Configure a strong password policy

## Policies

- MFA (Multi Factor Authentication) enabled on root and privliged IAM users
- Use principle of least privilege
- Use policy conditions, e.g. must have MFA

## Groups and Roles

- Use groups instead of assigning policies directly to users
- Use a group for every job function
- Use roles for application (Service or Delegated). No need for service accounts.
- Use roles for Delegation and Federation

## Monitoring

- Credential Report
- Access Advisor
- AWS CloudTrail
- AWS Trusted Advisor
- AWS Config

See [here](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html) for more details