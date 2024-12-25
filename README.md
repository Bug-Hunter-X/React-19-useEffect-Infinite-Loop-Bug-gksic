# React 19 useEffect Infinite Loop Bug

This repository demonstrates a common bug in React 19 involving the `useEffect` hook.  The bug causes an infinite loop due to a missing dependency array, leading to performance degradation.  The solution shows how to fix this by correctly specifying the dependencies.

## Bug
The `bug.js` file contains a component with an `useEffect` hook that lacks a dependency array. This causes the effect to run after every render, creating an infinite loop and flooding the console with log messages.

## Solution
The `bugSolution.js` file provides the correct implementation by including `count` in the dependency array. This ensures the effect only runs when the `count` value changes.