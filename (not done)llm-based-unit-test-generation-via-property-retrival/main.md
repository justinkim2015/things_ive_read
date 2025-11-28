# LLM-based Unit Test Generation via Property Retrieval
https://arxiv.org/pdf/2410.13542

## Overview
Current LLM-based unit test generation tools tend narrow their focus too much to only general code context, rather than looking at task-specific context and leveraging existing tests in unit test generation tasks. Additionally, the main metric being targetted is code coverage, at the expense of practical usability, correctness, and maintainability.

This paper proposes `Property-based Retrival Augmentation` which is a mechanism that extends RAG.  It accounts for the unique structure of unit tests by dividing the test generation phase into Given, When, and Then phases.  This forms property relationships between focal method and other methods, thereby expanding the scope of retrieval beyond traditional RAG.  Additionally, while creating tests, newly generated tests guide the creation of subsequent tests.

## Key Questions
1. How can we develop a retrieval mechanism that leverage task-specific information, such as considering esiting test cases in the context of unit test generation, to enhance LLM-based code generation for specific tasks?

2. How can we develop an appraoch that not only maximizes coverage but also produces unit tests that are correct, highly understandable, and maintainable?

### Solution
Rather than simply focusing on the code under test, the static context of the code (variables, function references) and existing test cases are also included.  By defining property relationship the context retrieval for LLMs is extended.  For each step of a unit test, Given, When, Then, the algorithm searchs for methods that provide insights to test generation based on the characteristics of the phase.

> A unit test is being generated for a method named `decode`.  A test case for a method called `encode` exists.

- Given Phase: The `encode` test case provides object setup information which can be referrenced for `decode` as the methods have similar data structures.
- When Phase: 
- Then Phase:
