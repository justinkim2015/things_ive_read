# Services: Great and Small

- Are services strongly decoupled? Not always.
- Do services allow independent development and deployment? Sometimes.

## Service Architecture?
- Just by using microservices, doesn't mean it's an architectural decision.
- Similar to how functions can simply separate behavior from each other, unrelated to The Dependency Rule, so can microservices.

## Benefits?

### Decoupling Fallacy
- Services can be strongly coupled due to the data they share.
- The interfaces are well defined, however, this is also true for functions in a monolithic application so this benefit is overstated.

### The Fallacy of Independent Development and Deployment
- As services are not necessarily loosely coupled (or decoupled completely), services cannot always be independently developed, deployed, and operated.
- To the level of coupling coming from data or behaviors, the development and deployment must also be coordinated.

### The Kitty Problem
- This taxi service is an example of a tightly-coupled microservices architecture.
- If they add a new service, for example, kitty delivery, they must change ALL microservices in order to make it work.

![kitty](kitty.jpg)

#### Component-Based Services
- This problem can be solved by having each service designed with clean architecture and SOLID principles.
- By adding new components and objects into the existing services, we can handle cross-cutting concerns. 

## Takeaway
- Services are useful for scalability and ease of development, however, they are not architectural elements by themselves.  The architecture is determined by boundaries drawn within the system.
