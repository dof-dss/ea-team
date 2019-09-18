# Gov.UK PaaS Hosting Model for DoF DSS

The chosen DoF DSS model for deploying enterprise services to the Gov.UK platform is for each service to be contained within its own Org. Each additional org has multiple spaces. Spaces represent environments that are appropriate for the service.

The main DoF DSS Org is used by DoF DSS to develop, test and run services owned and operated by DoF DSS which are not enterprise services.

![DoF DSS Hosting model](/docs/images/GovUKPaaS-Model-Simple.png)

This model has the following advantages:

* it is easy to manage user permissions with each org because spaces that require higher permissions (such as staging or production) are already separated from other spaces that do ot have as high a requirement
* developers that do not have security clearances yet can have their access restricted if necessary
* each org represents a business area which makes billing administration simple.

