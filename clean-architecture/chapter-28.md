# The Test Boundary

## Tests and System Components
- Tests follow the Dependency Rule, they depend inwards to the code being tested.
- They are the most isolate system component
- Their role is to support development

## Design for Testabiity
- As tests are generally isolated, develops tend to think they are not part of the system, **THIS IS INCORRECT**.

### Fragile Tests Problem
- Tests that are strongly coupled to the system must change along with the system. 
- Fragile tests make the system rigid, as small changes will break many tests, developers resist making changes.
- The solution is to design for testability, ex: tests that test the GUI are volatile, therefore find a way to test your business logic without testing the GUI.

## The Testing API
- You can create a specific API that tests can use to verify all the business rules.
- This allows you to decouple the tests from the application.

### Structural Coupling
- If a test suite has a test class for every production class and a set of test methods for each production method, the test suite is deeply structurally coupled.
- If anything changes, a large number of tests must change as well, making the tests fragile.

## Takeaway
- Tests are part of the system and the system must be designed to include them.  If they are not designed as part of the system, they tend to be fragile and difficult to maintain.