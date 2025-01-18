# Groovy NullPointerException in List Iteration
This example demonstrates a common error in Groovy when iterating through a list that may contain null values.  The `NullPointerException` occurs when the code attempts to access a member (in this case, implicitly using the `println` statement) of a `null` object.

## Bug Report
The `myMethod` function iterates through a list of integers. If a `null` value is encountered, a `NullPointerException` is thrown because Groovy does not automatically handle null values gracefully in this type of iteration. 

## Solution
The solution addresses the issue by explicitly checking for `null` values before attempting to process them.  This prevents the `NullPointerException` from being thrown.