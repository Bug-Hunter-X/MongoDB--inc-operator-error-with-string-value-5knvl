# MongoDB $inc Operator Error

This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations. The `$inc` operator is used to increment a numerical field by a specified value.  However, if you provide a string value instead of a number, the update operation will fail silently or produce unexpected results.

## Bug Description
The provided code snippet attempts to increment the `field1` in the `myCollection` by the string value '1'.  This is incorrect; the `$inc` operator requires a numerical value.

## Solution
The solution is to ensure that the value passed to `$inc` is a number. The corrected code is included in `bugSolution.js`.