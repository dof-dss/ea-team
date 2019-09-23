---
layout: default
title: Configuration repository and DEVOPS pipeline
---

# Implement documentation and configuration repository and DEVOPS pipeline

## Mission

The core objectives of this initiative are:

1. provide a central documentation repository for technical documentation in a collaborative environment,
2. provide a central configuration repository to allow configuration settings to be treated the same way as source code,
3. implement a devops pipeline (build/deploy/test) and support on-demand development/test environments

<hr />

## What problem are we solving

### Context

At present there is no unified way of handling software documentation. Software documentation is sporadic at best and non-existent at worst. When documentation does exist it is often hard to find and of varying formats and quality. Software configuration between environments is often a manual process and can lead to inconsistencies which makes identifying bugs before production more difficult. DevOps, and more specifically CI/CD pipelines are not common practice. Some teams use CI tools to varying degrees, others avoid them entirely and rely on purely manual process. The end result is that features ship late, are of low quality and are not easily maintainable by newcomers which leads to knowledge being held by a small number of team members.

### Personas

* Developers
* Operations
* Users
* Testers
* External Suppliers
* Contributors

### Scenarios

#### Scenario 1

A user rings the help desk to report an issue with one of their critical line of business systems. The system was developed by an internal development team several years ago. The organisation which has responsibility for supporting the system is notified of the issue and begin to investigate, however, the developers that originally worked on the software have moved on. The new developers tasked with investigating the solution have no experience with the technology or architecture the software was created in. The developers cannot find any documentation which details how to get the solution running locally so are unable to debug the issue easily. The development team also cannot find any documentation on what the software is supposed to do. The developers check logs to help identify where the issue might be, although due to the poor quality of the original solution the log messages are of little benefit.

The development team spend several days trying to reverse engineer the solution, eventually it is tracked back to a permissions issue on a feature the user is attempting to access. The issue is easily resolved by adding the user to the correct security group, the fix itself takes seconds to apply.

However, while the development team were attempting to find the cause of the issue the end user was prevented from completing a vital function within their business area, this caused them to miss their deadline for complying with a FOI request.

The development team also had to allocate their most skilled developers to investigate the issue. This caused a major update to a highly visible citizen facing service to be delayed which prevented the development team from delivering value to their customer.

<hr />

## How will we deliver this

We will move to a 'Code in the open' ethos, this means that everything we do will be publically visible and accessible. This will encourage transparency, accountability and collaboration.

We will migrate DoF DSS developers to GitHub

To effectively document our software all documentation will live with the code.
A core set of documents will be required for each product (service), these are:

1. Why did we build this?
  * Project Mission/background
2. What problem was it solving?
  * Project Context
  * Personas
  * Scenarios
3. How did we do it?
  * Architectural Design
  * Technical Documentation
4. Product Roadmap
5. How to deploy
6. How to run

We will migrate hosting of our products to the public cloud, specifically Gov.uk PaaS. This will facilitate faster provisioning of environments.

We will build CI/CD pipeline templates for Gov.uk PaaS hosted solutions.

## Roadmap

### Timeline

#### August 2019 to October 2019

{:class="table table-striped table-bordered"}
| Task | Description | Status |
| --- | --- | --- |
| `Create a DoF DSS Github Organisation` | Setup a Github Organisation for DoF DSS. All repositories should be open source. | Done |
| `Create a Contributor Code of Conduct` | As all repositories are open source it is important for the organisation to have a contributor code of conduct which clearly explains the repsonsibilities for all members of the organisation | Done |
| `Create a base repo template` | To ensure consistency a template repository should be created. This template repository should provide the common files and structure for all repositories to follow. | Done |
| `Setup Azure Pipelines` | Grant Azure Pipelines access to the repositories to allow CI/CD pipelines to be created | Done |
| `Setup Gov.uk PaaS access` | Get access to Gov.uk PaaS production platform | Done |
| `Setup DoF DSS Org on Gov.uk PaaS` | Create an organisation on Gov.uk PaaS for DoF DSS with sandbox, staging and production environments (spaces) | Done |
| `Configure Github access for on-prem CI/CD tools` | Allow tools such as Jenkins access to the organisation to allow for on-prem builds | In Progress |
| `Configure Github for Jira Integration` | Allow the Jira access to the organisation | Backlog |
