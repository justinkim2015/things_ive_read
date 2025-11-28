# Boundaries: Drawing Lines

## Boundaries
- Boundaries separate software elements from one another, and restrict those on one side from knowing about those on the other.

## What Boundaries and When?
- You should draw lines between things that matter and things that don't.
- ex: The GUI doesn't matter to the business logic, so therefore draw a line between them.

## Takeaways
- There were several anedotes about successful and unsuccessful architecture.  Generally the unsuccessful cases were a case of architects making pre-mature decisions, and the success story was how deferring the decision related to the data persistance method ended up with an easily extensible application that didn't have unnecessary development effort.
- Additionally, a lot of the chapter talked about boundaries and how they should be set.  Basically, if something can be interchanged, there should be a line or boundary drawn between these elements of the program.

