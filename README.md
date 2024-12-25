# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications where an infinite render loop is caused by incorrect usage of the `useEffect` hook.  The `useEffect` hook, while powerful, can lead to unexpected behavior if not used carefully.

The `bug.js` file contains the buggy code, while `bugSolution.js` provides the corrected version.

## Bug Description
The original code attempts to increment a state variable (`count`) within the `useEffect` hook, triggering an infinite loop because the state update causes the component to re-render, which, in turn, calls the `useEffect` again and again.