# Assessing Technical Debt

Every application naturally grows stale over time due to a number of different factors.  These factors all represent the accumulation of technical debt for an application.

## Factors that cause Technical Debt
1. Stale technology
An application grows stale as technology advances and the underlying technology used to implement the application moves on in terms of patches and upgrades.  This could be the tools, frameworks or languages used to create the application or any third party libraries the application is dependent upon are upgraded.  Falling behind in versions limits our agility and increases the maintenance and support burden by requiring more and more versions to be supported.  In more extreme cases it can result in an application leveraging a technology or tool that very few people have the skills or knowledge to maintain.  This presents a great risk that must be addressed as a matter of priority.

2. Application design and architecture
Applications should be constructed leveraging well known [software design patterns](https://en.wikipedia.org/wiki/Software_design_pattern) and [architectural patterns](https://en.wikipedia.org/wiki/Architectural_pattern).  Adopting these patterns ensures tried and tested solutions - that are well understood and are easily followed - are used to construct the application.  Poorly constructed applications are another form of technical debt because they too increase the support and maintenance burden due to requiring more time for developers to understand the uncommon workings of the application.

3. Limited reuse or sharing
Technical debt can also acrue if an application (or one of its dependencies) is superseeded or considered obsolete, perhaps due to a lack of desired functionality provided - even though the application may be using the latest technology upgrades and is, from a technical perspective, well designed and architected.  

4. Duplication of functionality
A related cause of technical debt is where multiple applications implement the same functionality.  This often arises when an application is implemented in a siloed way in departments and not in a way that allows reuse, either of the functionality or reuse/sharing of data.

5. Operational readiness
Applications have many non-functional requirements that should be satisfied in addition to delivering the functional requirements that result in the features and functionality required from the application.  Examples of non-functional requirements include logging, monitoring, availability, adoption of common data definitions and terms, etc.  Failing to implement non-functional requirements are another form of technical debt.


## Evaluating the degree of technical debt in an application
Technical Leads, Senior Developers or Architects will evalulate an application.  
Applications will be assessed against each of the above factors and scored using the following scale:- 

0 - No support for desired future state  
1 - Some support for desired future state  
2 - Much support for desired future state  
3 - Fully supports desired future state  

Scores for each factor will be added together to give a total overall score.  The possible total score for the technical debt of an application ranges from 0 (worst) to 15 (best).  Applications will be awarded Gold, Silver or Bronze based on its total score thus:-

Bronze :  0 -  5
Silver :  6 - 10
Gold   : 11 - 15

### My personal Thoughts / Queries / Objections to the suggested approach
- Is it too complicated?  Score 5 factors individually.  Total the scores.  Translate into gold/silver/bronze?  Converting to gold/silver/bronze is an attempt to summarise and simplify for architects and management, and also to gamify controlling tech debt.   Achieving gold standard sounds better than scoring 13/15.

- It's possible for an application written in, say modular-2 or VBA, to still achieve Gold standard if it's *really well* written, reusable and unique within NICS.  Should that be possible?
- It's possible for an application to be well written in the latest .Net Core version, etc but have zero reuse, and it still achieve a Gold standard.

- Should the Gold/Silver/Bronze be based on your lowest score?
- Should a 0 or 1 in any factor be an automatic bronze?

