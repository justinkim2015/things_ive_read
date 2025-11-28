# Policy and Level
- Software systems are statements of policy
- Policies will describe what the components of the system do (input validation, business logic, etc)
- Policies should be separated if they change for different reasons or at different times.

## Level
- A level is "The distance from the input and the outputs"
- The further a policy is from the input and outputs of the system, the higher its level.
- Policies that handle IO are the lowest-level policies in the system.
- Higher-level policies tend to change less frequently, and for more important reasons, than lower-level policies
- Lower-level polcies tend to change frequently, more urgently, but for less important reasons.

## Takeaways
- Low-level components are close to the IO and will often change. 
- High-level components should not depend on lower-level components.