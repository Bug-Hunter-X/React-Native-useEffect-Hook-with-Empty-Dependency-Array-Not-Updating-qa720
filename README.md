# React Native useEffect Hook Unexpected Behavior

This repository demonstrates a common error in React Native when using the `useEffect` hook with an empty dependency array (`[]`). The issue arises when the effect needs to react to changes outside the standard React component lifecycle, such as native module events or timers.  This example shows how to correctly handle such scenarios using the appropriate dependencies in the `useEffect` array.

**Problem:** The initial implementation of `useEffect` with an empty dependency array fails to update after receiving new data from a native module.  

**Solution:** The solution demonstrates incorporating the relevant data as a dependency in the `useEffect` array.  This ensures that the effect will run again whenever the data changes, resolving the unexpected behavior.