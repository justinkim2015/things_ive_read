# Object Oriented Programming (Re-read tomorrow)

What is OO?  
- The combination of data and function?
- A way to model the real world?
- The mixture of encapusulation, inheritance, and polymorphism

## Encapsulation
Encapsulation is considered a part of OO because OO languages provide easy and effective encapsulation of data and function.

This can be seen in things such as private data members and the public member functions of a class.

Can't really give this one to OO languages

## Inheritance
OO languages  made inheritance easier and multi-inheritence better.  
However, this was not brand new as there were hacks and tricks you could do in plain old C.

## Polymorphism
Polymorphism existed before OO languages.
However, OO languages made it much safer and easier to use polymorphism.

When using pointers outside of an OO language, you have to remember many things in order to make sure that the pointer is pointing to the right function.  Also, its dangerous as a bug here can be quite hard to track down.

**OO imposes discipline here on indirect transfer of control**

## Dependency Inversion
Before polymorphism was available, the flow of a calling tree would go a main level function -> high level function -> mid level function -> low level function.  They followed the **flow of control**.

```
What is "Flow of Control"?
In simple terms, the flow of control refers to the order in which instructions, statements, or function calls are executed within a program. It's the path that your program takes from its start to its end.

Traditional Flow: You have a fixed itinerary. You decide step-by-step where to go next.
Inverted Flow (DIP): You're given a map and a destination, but someone else (an abstraction) helps decide the specific route you take, or even what actions trigger the next step.
```

Therefore in order to call these lower level functions, you had to use an `include` or a `import`.

With polymorphism and interfaces, the high level function can call the function in a mid level function directly.
Additionally, the direction of the source code dependency changes to ML -> HL.

## Takeaways
Really OO is the ability through the use of polymorphism to gain absolute control over every source code dependency in the system.

It allows the architect to create a plugin architecture, in which modules that contain HL policies are independent of modules that contain low level details.

As the low level details will change often, these can be edited, changed, and plugged back into the high-level(HL) policies without changing the HL policies at all.