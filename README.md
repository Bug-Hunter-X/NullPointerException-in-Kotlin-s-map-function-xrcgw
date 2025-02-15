# Kotlin Map Function NullPointerException

This repository demonstrates a common error in Kotlin involving the `map` function and null collections.  The `BuggyMap.kt` file shows the problematic code that throws a `NullPointerException`. The `FixedMap.kt` file provides a solution using the safe call operator (`?.`) and the Elvis operator (`?:`).

## Problem

The `map` function in Kotlin throws a `NullPointerException` if the collection it operates on is null. This can be a subtle bug that's difficult to track down.

## Solution

The safe call operator (`?.`) allows you to safely call a method on a potentially null object. If the object is null, the expression short-circuits and returns null.  The Elvis operator (`?:`) provides a default value if the expression on the left is null.

By combining these operators, we can handle null collections gracefully and avoid the `NullPointerException`.
