# React useEffect Missing Return Statement
This repository demonstrates a common error in React applications involving the useEffect hook:  a missing return statement for cleanup functions.  Failure to return a cleanup function can lead to memory leaks and unexpected behavior, especially when dealing with subscriptions, timers, or event listeners.

## The Bug
The `bug.js` file shows an example of a component with a useEffect hook that lacks a return statement. This will likely cause a memory leak as the cleanup function is never called.

## The Solution
The `bugSolution.js` file provides a corrected version. It demonstrates the proper use of the return statement within the useEffect hook for cleanup.

## How to reproduce
1. Clone this repository.
2. Navigate to the directory using your terminal.
3. Run `npm install` to install the required dependencies.
4. Run `npm start` to start the development server.
5. Observe the console output.  Note that in the uncorrected version, the cleanup function is never called.