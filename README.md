# React useEffect Hook - Infinite Loop Bug

This repository demonstrates a common mistake when using the `useEffect` hook in React.  The `useEffect` hook is called after every render, causing an infinite loop. This example also demonstrates how to solve the issue by correctly specifying the dependency array.

## Bug
The bug is in the `MyComponent` function. The `useEffect` hook is called without the dependency array which makes it run after every render causing an infinite loop and performance issue. 

## Solution
The solution is to include the `count` variable in the dependency array. This ensures that the `useEffect` hook only runs when the `count` variable changes.