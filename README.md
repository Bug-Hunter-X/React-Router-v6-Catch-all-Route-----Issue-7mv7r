# React Router v6 Catch-all Route (*) Issue

This repository demonstrates a common issue encountered when using catch-all routes ("/*") in React Router v6.  The catch-all route unexpectedly intercepts all other routes, preventing proper navigation.

The `App.js` file contains the buggy code, while `AppSolution.js` provides a corrected version.

## Problem
The issue arises from the placement and usage of the catch-all route.  In this example, any route entered would lead to the NotFound component, even if other routes exist.

## Solution
The solution involves carefully ordering the routes. The catch-all route should always be placed last in the `Routes` component.