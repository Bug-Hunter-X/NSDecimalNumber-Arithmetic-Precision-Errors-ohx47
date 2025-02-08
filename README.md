# NSDecimalNumber Arithmetic Precision Errors in Objective-C

This repository demonstrates a subtle bug related to precision issues when using `NSDecimalNumber` for arithmetic operations in Objective-C.  The bug arises when performing calculations involving numbers of significantly different magnitudes.  While `NSDecimalNumber` is designed for precision, exceeding its limits can lead to inaccurate results.

The example code shows how small additions to large numbers can be silently ignored due to the internal precision limitations of `NSDecimalNumber`. This can cause logic errors in applications that rely on the exact results of these calculations.

The solution demonstrates safer approaches to handling `NSDecimalNumber` arithmetic to mitigate the precision issues and ensure correctness.