# React useEffect Hook Runs on Every Render Instead of Once

This repository demonstrates a common mistake when using the `useEffect` hook in React: the effect runs on every render instead of only once.  The provided code shows the bug and a solution.

**Bug:** The `useEffect` hook in `bug.js` is intended to log a message only once, on the initial render.  However, due to an incorrect dependency array, it runs on every render, resulting in excessive logging.

**Solution:** The solution in `bugSolution.js` corrects the issue by properly specifying an empty dependency array (`[]`), ensuring the effect runs only once after the initial render.

This example highlights the importance of carefully managing the dependencies in your `useEffect` calls.