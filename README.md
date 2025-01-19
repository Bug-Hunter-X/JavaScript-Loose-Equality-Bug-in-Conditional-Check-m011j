# JavaScript Loose Equality Bug
This repository demonstrates a common, yet subtle bug in JavaScript related to loose equality (==) within conditional checks. The bug arises when the function incorrectly treats 0 values as null, leading to unexpected results. The solution clarifies and provides a more robust approach for handling null and 0 values. 

## Bug Description
The provided `foo` function intends to return `null` only when either `a` or `b` is strictly `null`.  However, due to the use of loose equality (==), it also returns `null` when either `a` or `b` is 0, as `0 == null` evaluates to `true` in JavaScript.

## Solution
The solution employs strict equality (===) to correctly identify `null` values and handles 0 values appropriately. The revised function provides accurate results for all inputs, including 0 values.
