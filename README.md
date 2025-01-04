# React Router v6 - Missing 404 Route

This repository demonstrates a common error in React Router v6:  failure to include a catch-all route for handling 404 (Not Found) errors.  When a user navigates to a URL that doesn't match any defined routes, the application will crash.

The `bug.js` file showcases the problematic code, while `bugSolution.js` provides the corrected version.

## Problem

Without a catch-all route, React Router will not gracefully handle undefined paths, leading to an error in the console and a broken application.

## Solution

The solution involves adding a `Route` with a `path="*"` element that renders a 404 component. This route will match any URL that hasn't been explicitly defined.
