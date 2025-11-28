# The Database is a Detail
> From an architectural point of view, the database is a detail that does not rise to the level of an architectural element.

## Why are Database Systems so Prevalent?
- Reading from disk is slow.
- In order to fix this issue, we need indexes, caches, optimized query schemes and some means of representing the data.

## Why is it a Detail?
- The database is a mechanism we use to move the data back and forth between the disk and the RAM.
- We rarely use the data directly as we get it from the database, we transform it into whatever form we need.

## Takeaways
- While the actual technology of the database is indeed a detail, all it does is move data, the organizational structure of data **is** architecturally significant.
- The actual system that moves the data from a database to the RAM is a detail.
