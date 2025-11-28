# Chapter 2 - A Tale of Two Values

Each software system provides two different values to stakeholders, behavior and structure.

## Behavior
- This is how the machine behaves, done in a way to earn or save money for the stakeholders.
- This is done by creating a functional specification, then writing code that matches this spec.

## Architecture (Structure)
- Software must be soft and changable so that if requirements change, the program is easy to change.
- Effort should be proportional only to the scope of the change, not the shape of the change.
- Problems arise when stakeholders provide a stream of changes of a similar scope, however, due to increasing complexity of the architecture, the effort per feature increases.

## Important Takeaways
- Software engineers should fight for clean architecture
- A program without clean architecture will eventually become unchangable (due to costs)
- Architecture is more important then behavior -> If a program doesn't work and is easily changed, it can be quickly fixed, however if a program works but is unchangable, when the requirements change, it will be broken forever.