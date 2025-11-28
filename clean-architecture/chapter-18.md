# Boundary Anatomy

## Boundary Crossing
- A boundary crossing is a function on one side of a boundary calling a function on the other side and passing along some data.

## Monoliths
- A disciplined segregation of functions and data within a single processor and a single address space.
- "source-level decoupling mode"
- In this case a boundary crossing is simply a function call from a low-level client to a higher-level service.

## Deployment Components
- The simplest representation of a physical boundary is a library like a .Net DLL, a jar file, a Ruby Gem, etc...
- "Deployment level decoupling mode"

## Services
- This is the strongest boundary is a service.
- "Service level decoupling mode"
- Services are run independently of each other and communicate through the network.
- These are very slow

## Takeaways
- This chapter went into further depth about the three types of Boundary Modes.  It gave some more in-depth examples and explanations about these three modes.