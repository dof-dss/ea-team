---
layout: default
title: Groups
type: page
---
# IAM Groups: Definition
**An IAM group is a collection of IAM users**


## Things to note:
- No default IAM groups
- An IAM group is not a true identity
- Group names are unique across AWS account
- IAM policies can be attached to groups
- IAM users within an IAM group inherit all policies attached to group
- Groups cannot be nested
- An IAM user can be added to multiple groups
- Multiple policies can be attached to a group

## Best Practices
- Use groups as much as you can for flexible user management
- Evalute group policies and users on a regularr basis
- Apply policies to users directly sparingly