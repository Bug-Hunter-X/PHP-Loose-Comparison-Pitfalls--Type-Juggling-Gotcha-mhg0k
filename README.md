# PHP Loose Comparison Pitfalls

This repository demonstrates a common error in PHP related to loose comparisons and type juggling.  Loose comparisons (`==`) in PHP can lead to unexpected behavior due to automatic type conversion.  This example shows how a string value can be unexpectedly equal to a numeric value.

## The Bug

The `bug.php` file contains code that highlights this issue.  A string value ("0") is compared to an integer value (0) using a loose comparison.  The result is counter-intuitive for developers expecting strict type checking.

## The Solution

The `bugSolution.php` file provides a corrected version.  It uses strict comparison (`===`) to ensure both the value and the type match before execution.