# Unhandled Exception during JSON Decoding in Dart

This repository demonstrates a common error in Dart: neglecting to handle potential exceptions when decoding JSON responses from network requests.  The `bug.dart` file showcases the flawed code, while `bugSolution.dart` presents the corrected version.

## The Problem

The original code lacks proper exception handling around `jsonDecode`.  If the server returns invalid JSON or a network error occurs, the application crashes. 

## The Solution

The improved code includes a `try-catch` block to gracefully handle `FormatException` and other potential errors during JSON decoding.  This prevents unexpected application termination and allows for appropriate error reporting or fallback mechanisms.