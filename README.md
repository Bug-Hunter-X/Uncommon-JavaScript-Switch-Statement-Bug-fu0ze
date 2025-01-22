# Uncommon JavaScript Switch Statement Bug

This repository demonstrates an uncommon bug in JavaScript related to the use of switch statements and operator handling. The provided JavaScript code defines functions for basic arithmetic operations (addition, subtraction, multiplication, and division). It uses a switch statement to perform operations based on an operator symbol.  The primary bug lies in the lack of comprehensive error handling for invalid operator inputs.

## Bug Description
The initial code throws an error if an operator other than '+', '-', '*', or '/' is passed to the `operate` function. This error occurs because the switch statement doesn't include a `default` case to gracefully handle unexpected operators. This is an uncommon error because developers often overlook this scenario, expecting the switch statement to automatically handle such cases.

## Bug Solution
The solution improves the error handling by adding a `default` case to the switch statement. This `default` case intercepts any invalid operator, preventing a runtime error and providing a more user-friendly message.