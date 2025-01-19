# React Native Ref State Access Bug

This repository demonstrates a common issue in React Native where using refs to directly access a component's state can lead to unexpected behavior due to the asynchronous nature of state updates.  Accessing the state via ref immediately after an update might result in reading the old state value instead of the updated one. 

The `bug.js` file illustrates the problematic code.  The `bugSolution.js` file provides a solution using callbacks or effects to ensure proper state synchronization.

## How to Reproduce

1. Clone the repository.
2. Run `npm install`.
3. Run the app on a simulator or device.
4. Observe that the console log may show an outdated count value.