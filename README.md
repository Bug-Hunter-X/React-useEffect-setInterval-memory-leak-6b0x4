# React useEffect setInterval Memory Leak

This repository demonstrates a common bug in React applications involving the improper use of `setInterval` within the `useEffect` hook, leading to a memory leak.  The bug occurs because the interval is never cleared, causing the component to continuously update the state even after it's unmounted.  This results in wasted resources and potential performance issues.

The `bug.js` file contains the erroneous code.  The `bugSolution.js` file provides the corrected version, incorporating a cleanup function to clear the interval when the component is unmounted. 

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Observe the continuously incrementing counter.  This demonstrates the memory leak. 
5. Refer to `bugSolution.js` to see the corrected code.
