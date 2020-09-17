This project provides a memory efficient String implementation. Following brief explains the need for the same. 

Problem
------
Strings as immutable in Java. Java simplifies string manipulation operations by copying original string every time. However, it consumes memory. Especially, concatenate and split operations. We want to have a memory efficient string object without having to convert the whole program to C/C++.

Solution
-----
We will create a new string class that violates immutability but is represented by start and end pointer in a character array. Concatenate and split operations produce new objects with pointers in the same original character array.  For implementation(prototype) speed, I have used StringBuilder instead of character array. I will provide an alternative character array based implementation in future.
