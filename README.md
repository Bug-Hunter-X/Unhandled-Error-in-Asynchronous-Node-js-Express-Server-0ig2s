# Unhandled Error in Asynchronous Node.js Express Server

This repository demonstrates a common error in Node.js applications where an unhandled error in an asynchronous operation can cause the server to crash.  The `bug.js` file contains the problematic code, while `bugSolution.js` provides a corrected version with proper error handling.

## Problem
The original code simulates an asynchronous operation that might fail. If the operation fails, an error is thrown but not caught, leading to the server's termination.

## Solution
The solution involves using a `try...catch` block within the asynchronous operation to handle potential errors gracefully.  This prevents the server from crashing and allows for more robust error management.