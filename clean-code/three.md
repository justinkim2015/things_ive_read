# Functions

## Small!
- Functions should be small
- I personally disagree that they should be super tiny, but that's what is being reccomended

## Do One Thing
- Functions should do one thing. They should do it well. They should do it only.

## One level of abstraction per function
- The statements within our functino should be at the same level of abstraction.

## The Stepdown Rule
- We want each function to step down to the next level of abstraction

## Function Argument
- Ideally we want none to just a few arguments for our functions
- The reason being, it's hard to mentally track the arguments through the flow
- Additionally, this becomes harder to test as we need to test the various combinations of the arguments
- If you have a large number of arguments, it's often a sign that it should be wrapped into a class of its own.

## Have no side effects
- Methods need to do what it promises and only that
- Side effects are hidden things that your method is doing.

## Command query separation
- Functions should either do something or answer something, not both.
