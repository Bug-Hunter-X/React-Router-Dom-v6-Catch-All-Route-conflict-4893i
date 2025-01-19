# React Router Dom v6 Catch All Route conflict
This repository demonstrates a common issue in React Router Dom v6 where a catch-all route (`/*`) conflicts with other routes, preventing them from being matched correctly. The catch-all route unintentionally catches all other routes, leading to unexpected behavior.

## Problem
The provided code shows a basic React Router setup with a Home, About and a catch all NotFound component. The catch all route is defined to match any path that is not explicitly defined. However, this causes all routes to be matched by the catch all route.

## Solution
The solution involves reordering the routes, placing the catch-all route at the end of the routes array to ensure that it only matches routes that aren't explicitly defined.