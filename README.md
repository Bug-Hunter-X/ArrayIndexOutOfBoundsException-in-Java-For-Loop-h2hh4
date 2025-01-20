# ArrayIndexOutOfBoundsException in Java

This repository demonstrates a common error in Java: the `ArrayIndexOutOfBoundsException`. The error occurs when a program attempts to access an array element using an index that is either negative or greater than or equal to the array's length.

The `BuggyArray.java` file contains the code that throws the exception. The `FixedArray.java` file shows the corrected code. 

## How to reproduce the error

1. Compile the `BuggyArray.java` using a Java compiler: `javac BuggyArray.java`
2. Run the compiled code: `java BuggyArray`

You will see an `ArrayIndexOutOfBoundsException`.

## Solution

The problem lies in the `for` loop condition. It should be `i < arr.length` instead of `i <= arr.length`.  The corrected code is in `FixedArray.java`.