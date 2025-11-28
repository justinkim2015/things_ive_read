# Business Rules
- Business rules are rules or procedures that make or save the business money.
- Critical business rules are business rules that would exist even if there were no system to automate them.
- Critical business data is data that would exist related to the critical business rules.

## Entities
- This is an object within our system that embodies a small set of critical business rules operating on critical business data.
- Entities either contain critical business data, or has very easy access to that data.
- Entities are relatively pure in the sense that they would exist whether or not an automated system exists

## Use Cases
- Sometimes there are business rules that need to exist only in an automated system.
- These rules would not be used in a manual environment.
- These business rules that only are used in an automated system are called "Use Cases".
- They do not describe how the system appears to the user, instead they describe the application-specific rules that govern the interaction between the users and the entities.

## Request and Response Models
- Use cases expect input data and produce output data, however, this use case object shouldn't know HOW the data is being communicated.
- Use cases will recieve data structures and output data structure simply.

## Takeaways
- This chapter explained how business rules relate to entites and use cases, two commonly seen objects in a codebase.  Additionally, it introduced the concept of "Critical Business Rules/Data"