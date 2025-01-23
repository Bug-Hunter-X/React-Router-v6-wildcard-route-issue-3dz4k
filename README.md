# React Router v6 Wildcard Route Issue

This repository demonstrates a common issue encountered when using wildcard routes ('*') in React Router v6. The catch-all route intended to handle invalid paths is not functioning as expected.  The provided code includes a solution and explanation.

## Issue

When navigating to a non-existent route, the `NotFound` component does not render. Instead, React Router seems to ignore the wildcard route entirely.

## Solution

The issue is often related to the order of routes within the `Routes` component. The wildcard route (*) must be placed *last* to correctly catch any remaining paths. 