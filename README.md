# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook. The bug is caused by an infinite render loop due to a missing or incorrect dependency array in the `useEffect` hook.

## Bug Description

The `useEffect` hook in the provided `bug.js` file is missing a dependency array. This means that the effect runs on every render, causing the `count` state to constantly update, triggering another render, and creating an infinite loop.

## Solution

The `bugSolution.js` file demonstrates the fix. By including `[count]` as the dependency array, the effect only runs when the `count` value changes, resolving the infinite loop issue.
