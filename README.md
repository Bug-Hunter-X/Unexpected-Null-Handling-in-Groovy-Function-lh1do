# Groovy Null Handling Bug

This repository demonstrates a common issue in Groovy related to how null values are handled implicitly when they are passed to functions.  Groovy's flexible typing can mask potential errors if not explicitly addressed.

## Problem

The `calculate` function in `bug.groovy` is designed to add two numbers. However, it doesn't explicitly handle cases where one or both inputs are null.  This results in the function returning 0 instead of throwing an error or otherwise signaling the problem.

## Solution

The `bugSolution.groovy` file provides an improved version of the `calculate` function that explicitly checks for null values and throws an `IllegalArgumentException` if they are present. This makes the error handling more robust and prevents unexpected behavior.

## How to Run

1. Clone this repository.
2. Run the Groovy scripts using the `groovy` command: 
   ```bash
groovy bug.groovy
groovy bugSolution.groovy
   ```