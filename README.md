# React Memory Leak Bug

This repository demonstrates a common React bug involving memory leaks due to the improper use of `setInterval` within the `useEffect` hook.  The bug involves failing to properly clear the interval when the component unmounts, leading to continued execution of the interval even after the component is no longer needed.

The `bug.js` file contains the buggy code. The `bugSolution.js` file demonstrates the correct way to handle this situation by using `clearInterval` to clean up the interval before the component unmounts.