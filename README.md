# React Router DOM - Multiple BrowserRouter Instances

This repository demonstrates a common error in React Router DOM v6 and later, involving multiple `BrowserRouter` components.  The `Routes` component must be nested within a single `BrowserRouter`.  Having multiple causes unexpected routing behavior.

## The Problem

Incorrectly nesting `BrowserRouter` components results in the `Routes` component losing its context and causing unpredictable routing. This often manifests as routes not rendering or unexpected navigation behavior. The bug example shows the incorrect implementation. 

## The Solution

The solution ensures only one `BrowserRouter` wraps the application's routes and components.

## How to Reproduce

Clone the repository and run `npm install`. Then run `npm start` to see the error in the bug.js example. The solution demonstrates the corrected implementation. 