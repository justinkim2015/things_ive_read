# Functional Programming
In functional programming variables do not vary.

## Immutability and Architecture
Why is this important?

All race condtions, deadlock conditions, and concurrent update problems are caused by mutable variables.

You must ask yourself, if variable immutability is practical.  If you have infinite processor speed and storage the answer is yes, otherwise it is more nuanced and other compromises must be made.

## Segragation of mutability
One of the most common compromises regarding mutabiity is to segregate the app into mutable and immutable components. (stateful vs stateless).  If possible, one should do as much processing as possible into the immutable components to have less code in the mutable ones.

## Event Sourcing
Event sourcing is a strategy wherein we store the transactions but not the state of the application.  This means that the application will be stateless and can be rebuilt to any stage of it's life through the application history.

## Takeaways
- Structure programming is discipline imposed upon direct trasnfer of control
- Object Oriented programming is discipline imposed upon indirect transfer of control
- Functional Programming is discipline imposed upon variable assignment.