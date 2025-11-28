# Structured Programming

## Proofs
- certain uses of goto statements made it so that modules couldn't be broken down into smaller and smaller units therefore making it hard to write proofs for.
- Some uses of goto (if/then/else and do/while) didn't have this problem.
- All programs can be constructed by 3 things:
1. sequence
2. selection
3. iteration

## Functional Decomposition
- As structured programming allowed modules to be recursively decomposed into provable units, large modules can be functionally decomposed.
- It involves recursively abstracting parts of a large module in a logical, top-down manner. Each decomposition reduces scope and complexity, making the components easier to reason about and test — ultimately helping to prove that they are not incorrect.

## Key Takeaways
- Tests prove a program is not incorrect, not that it is correct.
- Structured programming forces us to recursively decompose a program, then we can test these to prove the program is not incorrect.
- Functional decomposition is one of our best practices