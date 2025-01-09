# Incorrect State Update in React useEffect Hook

This repository demonstrates a common mistake in React: directly modifying state variables within the `useEffect` hook without using the `setState` function.  This leads to the state not updating correctly and no re-render happening.

The `bug.js` file contains the erroneous code. The `bugSolution.js` demonstrates the corrected approach.

## Bug:
Directly modifying the state variable `count` within the `useEffect` hook does not trigger a re-render. The component's display will not reflect the actual changes to the state variable.

## Solution:
Always use the `setState` function (`setCount` in this case) to update state variables.  This ensures that React's state management system is correctly notified, leading to the expected re-render.
