# DIP: The Dependency Inversion Principle

```
The most flexible systems are those in which source code dependencies refer only to abstractions, not to concretions.
```

- In statically typed languages, imports should only refer to source modules containing interfaces, abstract classes, or some other kind of abstract declaration.  Nothing concrete should be depended on.
- We can ignore very stable classes of the operating system and platform facilities when it comes to DIP.
- We must avoid dependencies on the volatile concrete elements of our system.

## Stable Abstractions
- Every change to an abstract interface corresponds to a change to its concrete implementations.  
- On the other hand, changes to a concrete implementation do not always require cahnges to the interfaces they implement.
- **Therefore interfaces are less volatile than implementations**

## Factories
- We can use factories to avoid direct dependency on high-level(business logic-like) code.
- We no longer directly depend on the concrete implementation, but rather the abstraction which is the factory.

## Takeaways
- We should not directly depend on concretions as they change often.
- Interfaces need to change much less, therefore they create more stable code.