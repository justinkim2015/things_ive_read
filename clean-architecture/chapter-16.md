# Independence

## Use Case
- This means the architecture of the system must support the intent of the system
- An application with good architecture will look like the application it is supposed to be.  Future developers will not have to hunt to find behaviors as they will be readily visible.

## Operation
- The architecture must support the non-technical needs of the system
- Operation related architecture decisions are often one that is left open until later as they are hard to change later.

## Development
```
# Conway's Law
Any organization that designs a system will produce a design whose structure is a copy of the organization’s communication structure.
```
- A system that must be developed by an organization with many teams and many concerns must have an architecture that facilitates independeant actions by those teams, so the teams don't interfere with each other during development.

## Deployment
- The goal is immediate deployment.

## Leaving Options Open
- The reality of development is that we often don't know all the requirements or the requirements will change.
- Good architecture makes the system easy to change in all the ways it must change.

## Decoupling Layers
- We can divide the system into decoupled horizontal layers--UI, business logic, database, etc...

## Decoupling Use Cases
- We can decouple use cases as certain use cases will change more or less than others.
- Adding new or changing use cases won't affect others.

## Decoupling Mode
- As we decoupled, use cases and layers, for operations different components will also need different non-technical requirements.
- These often must be independent services running on their own server and that communicate over a network.
- "Service-oriented architecture" (SOA)
### Source Level 
- Monolith
- We control the dependencies between source code modules

### Deployment Level
- We control the dependencies through deployable units such as DLLs, jar files, or shared libraries.

### Service level
- We run each dependency independently and communicate through packets.
- Microservices

## Independent Develop-Ability
- As long as the layers and use cases of the system are decoupled, each team will not impede each other while developing their features.

## Independent Deployabiity
- If the decoupling is done well, it should be possible to deploy different layers independently of each other.

## Duplication
- True duplicates vs false/accidental duplication
- True duplication must be avoided.
- When things change at different rates or for different reasons, this is false duplication and is fine.

