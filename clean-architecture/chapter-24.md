# Partial Boundaries
- Full boundaries are expensive, sometimes a partial boundary might be better.

## Skip the Last Step
- A way to construct a partial boundary is to do all the work necessary to create independently compilable and deployable components, then keep them together in the same component.
- This requires the same amount of code and design work as a full boundary, however, there is no admin of multiple components such as version numbers or release management.

## One-Dimensional Boundaries
- Full boundaries are reciprocal, they maintain isolation in both directions.
- A one-dimensional boundary holds the place for later extension to a full-fledge boundary.
- We create a service boundary interface which will later be replaced with a proper interface in the case it is needed.
![alt text](service_boundary.jpg)

## Facades
- The Facade class lists all serices as methods and deploys the service calls to calsses that the client is not supposed to access.

![alt text](facades.jpg)

## Takeaway
- There are several ways to partially implement an architectural boundary.  Each has its trade-offs and they must be considered when picking one.