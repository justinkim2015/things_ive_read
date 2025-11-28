# LLM-based Unit Test Generation via Property Retrieval
https://arxiv.org/pdf/2410.13542

## Overview
Current LLM-based unit test generation tools tend narrow their focus too much to only general code context, rather than looking at task-specific context and leveraging existing tests in unit test generation tasks. Additionally, the main metric being targetted is code coverage, at the expense of practical usability, correctness, and maintainability.

This paper proposes `Property-based Retrival Augmentation` which is a mechanism that extends RAG.  It accounts for the unique structure of unit tests by dividing the test generation phase into Given, When, and Then phases.  This forms property relationships between focal method and other methods, thereby expanding the scope of retrieval beyond traditional RAG.  Additionally, while creating tests, newly generated tests guide the creation of subsequent tests.