# What is Architecture
- The Architecture of a software system is the shape given to that system by those who build it.
- The form of the shape is in the division of that system into components, how the components are arranged, and the ways in which those components communicate with each other.

## Purpose of Architecture
- The purpose is to faciliate the development, operation, and maintenance of the software system contained within it.
```
Leave as many options open as possible, for as long as possible.
```

## Development
- A software system that is hard to develop is not likely to have a long and healthy lifetime.
- Architecture is also effected by team structures, a small team is less likely to need a strict form at the start, where a large team would.

## Deployment
- The higher the cost of deployment, the less useful a system is.
- A goal of architecture should be to make a system that is easily deployed with a single action.

## Operation
- Architecture's impact of operation is comparatively lower.
- This is because operation issues can be often solved by increasing specs.
- However, architecture should make the operation of the system readily apparent to the developers.  It should be easy to see how the system is supposed to be used.

## Maintenance
- Maintenance is the most costly aspect of a system.
- The primary costs of maintenance are spelunking and risk.
- Spelunking: The cost of digging through the existing code to find how to fix a bug or add a new feature.
- Risk: The risk of making changes to an already working system

## Takeaways
- Architecture is about the development, deployment, and maintenance of a system.
- By separating and decoupling details from policy, we can hold off on actually deciding the details for as long as possible.  This allows us to be flexible and make better decisions.

