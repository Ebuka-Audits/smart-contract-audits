
```md id="notes1"
# Reentrancy Notes

## Key Idea
Reentrancy occurs when a contract makes an external call before updating its internal state.

## Rule
Always follow:
Checks → Effects → Interactions

## Dangerous Pattern
- External call before state update

## Safe Pattern
- State update before external call

## Real Insight
Security must apply to ALL functions, not just main ones.
