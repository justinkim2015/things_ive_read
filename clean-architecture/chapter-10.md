# ISP: The Interface Segregation Principle

```
No could should be forced to depend on methods it does not use
```

- If user A only uses operation A and user B only uses operation B, but they both are in class A, any change to either will result in having to recompile and redeploy the whole thing.
- This can be solved by only exposing the parts each user uses through interfaces

## ISP and Architecture
- In general it's harmful to depend on module that contain more than you need.

## Takeaways
- Don't depend on things you don't need.