# The Main Component
- In every system there is one component that creates, coordinates, and oversees the others.  This is called the main component.

## The Ultimate Detail
- This is the lowest level policy, the initial entry point into the system
- It should use a DI framework to inject all the dependencies
- This is the dirtiest lowest level module which simply sets up everything for the higher level system, then hands over control.

## Takeaways
- Main is simply the entry point to the system where you have to set everything up and then pass it to the rest of the program.