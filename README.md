# MongoDB $inc Operator Error
This repository demonstrates an error caused by the incorrect use of MongoDB's `$inc` operator. The `$inc` operator is used to increment a numeric field by a specified value.  However, in the provided code, a string value is being used, resulting in unexpected results.

## Bug Description
The bug stems from attempting to increment a field using a string value in the `$inc` operator.  MongoDB expects a numeric value, not a string. This leads to an update operation that might not produce the intended results or could even throw an error.

## Solution
The solution involves providing a numeric value to the `$inc` operator, correcting the data type of the value.