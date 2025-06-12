<p align="center">
  <img src="https://github.com/Chill-Astro/OpenScan/blob/main/OpenScan.png" width="540px">
</p>
 
OpenScan is a robust, efficient, and versatile Java library designed to replace the standard Scanner class for handling user input. It offers significant advantages in terms of performance, error handling, and flexibility, especially when dealing with large inputs or complex data formats.

---

## Getting Started :

1.  **Download :** Clone or download the `OpenScan.java` file from this repository.
2.  **Include :** Add the `OpenScan.java` file to your Java project.
3.  **Create Object :** Create an Object from this Code :

    ```java
    OpenScan <object-name> = new OpenScan();
    ```
    ↑ - This allows you to access the non-static methods only!
---

## Usings :
 
- Assuming sc is the object, the following methods are available:

   * sc.next() -> Reads the next token as String
   * sc.nextLine() -> Reads the next line as String
   * sc.nextInt() -> Reads the next token as int
   * sc.nextLong() -> Reads the next token as long
   * sc.nextDouble() -> Reads the next token as double
   * sc.nextFloat() -> Reads the next token as float
   * sc.nextBoolean() -> Reads the next token as boolean
   * sc.nextShort() -> Reads the next token as short
   * sc.nextByte() -> Reads the next token as byte
   * sc.nextChar() -> Reads the first character of the next token
   * sc.hasNext() -> Checks if another token is available
   * sc.nextIntArray(n) -> Reads n integers into an int[]
   * sc.nextLongArray(n) -> Reads n longs into a long[]
   * sc.nextDoubleArray(n) -> Reads n doubles into a double[]
   * sc.nextStringArray(n) -> Reads n tokens into a String[]
   * sc.nextIntMatrix(r, c) -> Reads r x c integers into int[][]
   * sc.nextDoubleMatrix(r, c) -> Reads r x c doubles into double[][]
   * sc.nextStringList() -> Reads all remaining tokens in the current line as List<String>
   * sc.nextStringListLine() -> Reads all tokens from the current/new line as List<String>
   * sc.skipLines(n) -> Skips n lines
   * sc.readAllLines() -> Reads all lines as List<String>
   * sc.readUntil(delim) -> Reads tokens until delim is found (not included)
   * sc.peek() -> Peeks at the next token without consuming it
   * sc.readAllInts() -> Reads all remaining tokens as List<Integer>
   * sc.readAllDoubles() -> Reads all remaining tokens as List<Double>
   * sc.readAllLongs() -> Reads all remaining tokens as List<Long>
   * sc.readAllStrings() -> Reads all remaining tokens as List<String>
   * sc.close() -> Closes the input reader

 - Static Methods that are also available [no object needed] :

   * OpenScan.fromFile(path) -> Creates OpenScan from file
   * OpenScan.fromString(str) -> Creates OpenScan from string

---

## Key Features and Advantages :

*   **Enhanced Performance:**
    *   Leverages `BufferedReader` for efficient line-by-line reading.
    *   Uses buffering to reduce the number of physical read operations, resulting in faster I/O.
*   **Line-Oriented Input:**
    *   `nextLine()` method efficiently reads entire lines, unlike `Scanner`'s token-based approach.
*   **Robust Error Handling:**
    *   Explicitly throws `NoSuchElementException` when input is exhausted.
    *   Throws `NumberFormatException` for invalid numeric input.
    *   Throws `RuntimeException` (wrapping `IOException`) for I/O errors.
    *   Handles empty tokens when `nextChar()` is called.
*   **Automatic Resource Management:**
    *   Implements `AutoCloseable`, allowing for use with try-with-resources, ensuring proper resource cleanup.
*   **Comprehensive Data Type Support:**
    *   Directly reads various data types: `int`, `long`, `double`, `float`, `boolean`, `char`, `short`, `byte`.
*   **Flexible Array, Matrix, and List Reading:**
    *   `nextIntArray(n)`, `nextLongArray(n)`, `nextDoubleArray(n)`, `nextStringArray(n)` read multiple values into arrays.
    *   `nextIntMatrix(r, c)`, `nextDoubleMatrix(r, c)` read 2D arrays (matrices) of input.
    *   `nextStringList()` reads all tokens on the current line into a `List<String>`.
    *   `nextStringListLine()` reads all tokens from the current or new line as a `List<String>`.
    *   `readAllLines()` reads all lines as `List<String>`.
*   **Complete Data Loading:**
    *   `readAllInts()`, `readAllDoubles()`, `readAllLongs()`, `readAllStrings()` read all available data from the input stream.
*   **Input Control:**
    *   `skipLines(n)` efficiently skips over unwanted lines of input.
    *   `readUntil(delim)` reads tokens until a delimiter is found.
*   **Peeking and Tokenizer Control:**
    *   `peek()` allows peeking at the next token without consuming it.
    *   `nextLine()` method clears the tokenizer by assigning null.
*   **Robust Checking:**
    *   `hasNext()` method checks properly if a new token is available.
*   **Detailed Exception Handling:**
    *   Handles all exceptions clearly.

---

## Note from Developer :

Appreciate my effort? Why not leave a Star ⭐ ! Also if forked, please credit me for my effort and thanks if you do! :)

---
