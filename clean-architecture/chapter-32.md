# Frameworks are Details

## Framework Authors
- Framework authors solve their own problems, not yours.

## Asymmetric Marriage
- When you adopt a framework, you must made a huge commitment to the framework, however, the framework makes no commitment to you.
- In practice this means that you will be tightly coupled to the framework you adopt.

## The Risks
- The architecture of frameworks often violate The Dependency Rule as you inherit their code into your Entity domain.
- The framework may help early but restrict you later on.
- The frameway may change in a way you don't find helpful.
- A new framework may come along that you wish to change to.

## The Solution
> Don't marry the framework!

- Use the framework but don't couple your code to it.
- Treat the framework as a detail that exists in the outer layers of the architecture.

## Takeaways
- When using frameworks try your best to not couple them strongly to your application.
- Keep the framework in the outermost layers of your architecture.
