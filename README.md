# React useEffect Infinite Render Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook. The bug results in an infinite render loop, causing the application to become unresponsive.

## Bug Description

The provided code includes a `useEffect` hook that runs after every render without specifying any dependencies.  This leads to an endless cycle of rendering and updating the component state.

## Solution

To fix this issue, the `useEffect` hook needs to include an empty dependency array `[]` to ensure it only runs once after the initial render, as shown in `bugSolution.js`.