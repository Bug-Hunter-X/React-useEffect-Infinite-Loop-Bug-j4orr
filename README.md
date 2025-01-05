# React useEffect Infinite Loop Bug
This repository demonstrates a common React bug involving the `useEffect` hook.  The component falls into an infinite loop due to a missing dependency in the `useEffect` call. The solution showcases how to correctly specify dependencies to resolve this issue.

## Bug
The `bug.js` file contains the buggy component.  It uses `useEffect` to log the count, but the `count` state variable is missing from the dependency array, resulting in an infinite render loop.

## Solution
The `bugSolution.js` file provides the corrected component. By including `count` in the dependency array, the effect only runs when the `count` variable changes, preventing the infinite loop.

## How to reproduce
1. Clone this repository
2. Run `npm install`
3. Run `npm start`
Observe the behavior of the buggy component, then compare to the corrected version.