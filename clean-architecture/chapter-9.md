# LSP: The Liskov Substitution Principle

If you have a base type and a subtype (a derived class), you should be able to use an object of the subtype anywhere an object of the base type is expected, without breaking the program.

## LSP and Architecture
The best way to understand the LSP from an architectual point of view, is to see what happens when it is violated.

**Example**
We have a taxi service that can dispatch cabs from several different companies.  

If one taxi company (ACME taxis) used a different response type what do we do?  
-> We'd have to make a special case obviously.

Because these are not all the same and interchangable, we have to include a lot more complexity to make it work.

## Takeaways
- LSP can and should be extended to the level of architecture.
- A violation of substitutability can cause a system's internals to become unnecessarily complex.


