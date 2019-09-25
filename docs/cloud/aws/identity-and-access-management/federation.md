---
layout: default
title: Federation
type: page
---

# Federation
Federation enables you to manage access to your AWS Cloud resources centrally. With federation, you can use single sign-on (SSO) to access your AWS accounts using credentials from your corporate directory or social identities.

## Benefits
- Single Sign On
- Centralized
- Security and Compliance

## Types
- Cross Account
  - between different AWS accounts
  - sts:AssumeRole
  
- Web Identity
  - OpenId (Amazon, Facebook, Google)
  - integrates with Cognito
  - Users do not need AWS account
  - No need to maintain users
  - sts:AssumeRoleWithWebIdentity

- SAML2
  - Security Assertion Markup Language
  - Open standard used by many APIs: OAUth, MS AD Federation Service, etc
  - sts:AssumeRoleWithSAML
  
- AWS Directory Services
  - Simple AD
  - AWS for Microsoft AD
  - AD connector

**IAM role assigns temp permissions and these roles are assumed by perople or applications**


