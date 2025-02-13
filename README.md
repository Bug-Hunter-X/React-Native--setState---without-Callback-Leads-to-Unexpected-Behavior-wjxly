# React Native setState() Issue
This repository demonstrates a common issue in React Native applications: using the `setState()` method without a callback function, which can result in incorrect state updates. The `bug.js` file shows the incorrect implementation, while `bugSolution.js` provides the corrected version.

The problem arises when the state update depends on the previous state value. Without the callback, the update might use a stale state value, leading to unexpected behavior.

The solution is to always use a callback function with `setState()`, to ensure that the update is based on the current state.