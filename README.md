# React Router v6 Catch-all Route Issue

This repository demonstrates a common issue encountered when using catch-all routes (`/*`) in React Router v6.  The catch-all route unexpectedly intercepts all other routes, preventing them from being matched.

The problem stems from the order of routes within the `Routes` component.  The catch-all route should always be placed last to ensure it only matches paths not covered by more specific routes.  This example highlights the correct and incorrect implementations. 

## Solution
The solution involves placing the catch-all route (`/*`) after all other defined routes.  See `AppSolution.js` for the corrected version. 