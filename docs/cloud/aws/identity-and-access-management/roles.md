---
layout: default
title: Roles
type: page
---
# IAM Roles
## Things to Note:
- Another AWS Identity
- Policies are attached to roles
- Roles are assumed by user, applications and external users

## Benefits
- No long term credentials
- No need to embed permanent credentials into an application
- No need for IAM user creation
- Easily federate external users

## Policy Types
- Permission Policy: Define whats actions and resources the role can use
- Trust Policy: Define who is allowed to assume a role

## AWS Security Token Service (STS)
IAM roles rely on STS to:
- Provide temporary security credentials
- Short term credentials from 15 mins to 36 hours
- Credentials are dynamically assigned as requested
- No need to rotate / revoke passwords or access keys

## Service Role
AWS service assumes role on behalf of application, e.g. create a service role for EC2 instance, add a S3 access policy to it and attach to instance: Now any application on that instance can access S3 bucket without need to embed credentials in application.

## Delegated Role
Allows different AWS accounts to access resources.
    - Trusting: account with resources
    - Trusted: User in other AWS account

## Federated Roles
Two types of federated roles:
    - SAML 2 Federation
    - Web Identity Fedearation: e.g. Amazon, Google, Facebook
Both types require a trust relationship between account and identity providers

## IAM Roles: Best Practices
- Use roles for applications, instead of creating IAM users
- Use roles for exisitng corporate identities instead of creating multiple identities
- Use roles for web identities requiring temporary access
  