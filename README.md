# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook.  The bug arises from an incorrect dependency array, leading to an infinite rendering loop.

## Bug Description
The `useEffect` hook is used to perform side effects after a component renders.  If the dependency array is incorrect, the effect might run unexpectedly, causing infinite loops and performance issues. In this example, omitting `count` from the dependency array causes the effect to run on every render, triggering a new state update, which in turn triggers another render, leading to an infinite loop.

## How to Reproduce
1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Observe the console and the infinite loop.