# Unhandled JSON Decoding Exception in Dart

This repository demonstrates a common error in Dart applications involving asynchronous operations and JSON decoding.  The `bug.dart` file contains code that attempts to fetch and decode JSON data from an API without proper exception handling.  This can lead to crashes if the API response is not valid JSON. The `bugSolution.dart` file provides a corrected version with improved error handling.

## How to Reproduce the Bug

1.  Clone this repository.
2.  Run `bug.dart`.  Observe that a `FormatException` is thrown if the API endpoint returns invalid JSON (or if there's a network error).

## Solution

The solution involves adding a `try-catch` block to gracefully handle potential exceptions during JSON decoding.  This prevents the application from crashing and allows for more robust error handling.