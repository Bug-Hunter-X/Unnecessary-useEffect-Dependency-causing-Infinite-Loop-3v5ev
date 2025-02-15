# Unnecessary useEffect Dependency causing Infinite Loop

This example demonstrates a common React bug where an unnecessary dependency in the `useEffect` hook causes an infinite rendering loop.  The `useEffect` hook is called after every render because the `count` variable is implicitly considered a dependency.  This leads to a continuous update cycle.

## How to reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the console output – you'll see the 'Count:' log endlessly.