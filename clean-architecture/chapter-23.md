# Presenters and Humble Objects

## The Humble Object Pattern
```
Split the behaviors into two modules or classes.  One module is humble, it contains all the hard-to-test behaviors stripped down to its barest essence.  Other other contains all the testable behaviors that were stripped out of the humble object.
```
- This is a pattern that was identified to help unit tests separate behaviors that are hard to test from those which are easy to test.

## Presenters and Views
### Views
- The view is the humble object that is hard to test.
- It moves data into the GUI but does not process that data

### Presenters
- Its job is to accept data from the application and format it for presentation so that the View can move it to the screen.

## Database Gateways
- These come between the use case interactors and the database.
- These are an interface that goes between the database (SQL) and the use cases.
- The database (SQL) is humble, as the business logic is extracted to the gateway, and therefore the business logic in the gateway is testable.

## Takeaways
- This section explained the humble object pattern and how using this pattern makes your code more testable.  
