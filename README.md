# React useEffect Hook Issue

This repository demonstrates a common error related to the `useEffect` hook in React. The component fails to update the document title when the count is decremented from 1 to 0 because of an incorrect condition in the useEffect dependency.

## Bug Description:

The `useEffect` hook is designed to perform side effects based on changes in component state or props. In this case, the component attempts to update the document title whenever the `count` changes. However, the condition `if (count > 0)` prevents the title update when the count goes from 1 to 0.

## Solution:

The solution involves modifying the condition within the `useEffect` hook to ensure the title updates even when the count decreases to 0.  The corrected condition checks if the count is greater than or equal to 0.

## How to reproduce the bug:

1. Clone this repository
2. Install dependencies: `npm install`
3. Run the application: `npm start`
4. Observe that the document title doesn't update when the counter decrements from 1 to 0.

## How to fix the bug:

Refer to the `bugSolution.js` file for the corrected implementation.