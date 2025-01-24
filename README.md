# React useEffect Hook Missing Dependency

This repository demonstrates a common error in React applications involving the `useEffect` hook: missing dependencies in the dependency array.  This can lead to unexpected behavior, including infinite loops and incorrect state updates.

## The Bug
The `bug.js` file contains a component that uses the `useEffect` hook to log the current count to the console.  However, the `count` variable is missing from the dependency array. This causes the effect to run after every render, regardless of whether the `count` has actually changed.

## The Solution
The `bugSolution.js` file shows the corrected code. By including `count` in the dependency array, the effect only runs when the value of `count` changes.

## How to reproduce
1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the development server.
5. Observe the console logs to see the difference in behavior between the buggy and corrected components.
