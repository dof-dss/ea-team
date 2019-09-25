# Expose APIs and message queues

## Statement
All data stores must be exposed via APIs.  All applications must provide APIs and/or message queues as standard to maximise reuse and interoperability.

## Rational
One of the biggest challenges in service delivery is standardised exchange of information to ensure that the same approach is used by a single service to get functionality or data from systems in different departments. 

## Implications
- When building systems, or new services, expose any functionality via APIs or queues and communicate with other services using message queues (where possible) or API calls (where sync exchange of data required).
- Guidance in the form of an API Style Guide must be published to ensure quality and standardisation of APIs.
- An enterprise service bus is required to support message transportation around the enterprise.
- [Common vocabulary and data definitions](./common-vocabulary-and-data-definitions.md) must be defined to ensure interoperability between systems.

[View list of all NICS Architecture Principles](../Architecture-Principles.md)