# Vibu - Java Code Example

## Overview

The `Vibu` class is a simple Java program that demonstrates the manipulation of a 3-dimensional integer array and the conversion of integer values to characters based on ASCII values.

### Functionality

1. **Initialization**: 
   - The program initializes a 3-dimensional array `a` with predefined values: `{{{1, 2}, {3, 4}}, {{5, 6}, {7, 8}}}`.

2. **Processing**:
   - The code iterates through each element of the 3D array.
   - For each element, it generates four different strings by adding various offsets (47, 48, 49, 50) to the integer values, and then converting these values to characters.

3. **Output**:
   - It prints four strings where each string is constructed by converting the array values with different ASCII value offsets.

## Code Explanation

The main logic of the code is contained in the `main` method:

- Array Initialization:
  ```java
  int[][][] a = {{{1, 2}, {3, 4}}, {{5, 6}, {7, 8}}};

 String Initialization:
String s = ""; 
String s0 = ""; 
String s1 = "";
String s2 = "";

Nested Loops:
for (int i = 0; i < 2; i++) {
    for (int j = 0; j < 2; j++) {
        for (int k = 0; k < 2; k++) {
            s = s + (char) (a[i][j][k] + 47); 
            s0 = s0 + (char) (a[i][j][k] + 48); 
            s1 = s1 + (char) (a[i][j][k] + 49);
            s2 = s2 + (char) (a[i][j][k] + 50); 
        }
    }
}
Output:   (The program prints the resulting strings with different ASCII offsets):
System.out.println("ASCII Value(47) Added with Arrays: " + s);
System.out.println("ASCII Value(48) Added with Arrays: " + s0);
System.out.println("ASCII Value(49) Added with Arrays: " + s1);
System.out.println("ASCII Value(50) Added with Arrays: " + s2);

