# React Native App Crash on Network Error

This repository demonstrates a common bug in React Native applications where an app crashes due to improper error handling during asynchronous data fetching.  The bug is caused by a missing error handling in a try...catch block within a useEffect hook. This example showcases the problem and its solution.

## Bug

The `bug.js` file contains the buggy component that crashes upon encountering a network error.

## Solution

The `bugSolution.js` file provides a corrected version of the component with robust error handling. The solution handles network errors gracefully and prevents the app from crashing by setting a default state or displaying an appropriate error message.

## How to reproduce

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install the dependencies.
4. Run `npx react-native run-android` or `npx react-native run-ios` to run the app.
5. Observe the crash when the network request fails (e.g., by intentionally disrupting the network connection).
6. Review the corrected code in `bugSolution.js` to learn how to implement proper error handling.