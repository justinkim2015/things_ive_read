# OCP: The Open-Closed Principle

```
A software artifact should be open for extension but closed for modification
```

In other words, the behavior of a software artifact should be extensible without having to modify that artifact.

## OCP Basics
Basically things in different layers are unidirectionally protected.
The functionality is separated based on how, why and when it changes.
**Higher level components are protected from changes from lower level components**

## Directional Control
We can use interfaces to invert the dependency between components.

## Takeaways
The goal is to make systems easy to extend.  This is accomplished by splitting the program into components and creating a dependency hierarchy that protect high-level components from changes in low-level components.