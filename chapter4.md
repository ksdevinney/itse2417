# Chapter 4: Data Types

## Constants

Good practice to reduce the number of literal numbers; use variables to replace use of literals

Constant variables (final variables) cannot be changed, usually named in ALL CAPS with underscores between_words

## Math Methods

Math class contains methods for various math operations (sqrt, abs, pow), do not need to import anything

## Integer Division and Modulo

Integer division: performed when both operands of / are integers, does not generate any fractions

Modulo: % evaluates the remainder of a division problem; can be used to get a random number, get digits of a number:

last digit = number % 10
temporary number = number / 10
and continue

Integer division by a power of 10 shifts the number to the right, modulo by power of 10 gets the last digit(s)

## Type Conversions

For integer operations where one value is a double, the other is automatically converted as well

Double-to-int conversions are not automatic due to loss of precision

You can also explicitly convert one type to another: (double) intVariable converts an int to a double

## Binary

rightmost digit is 2^0 (1), power continues to the left (2^3, 2^2, 2^1...)

## Characters

char data type stores one character, in single quotes

no method for getting a single character from input, must use next().charAt(0) to obtain the first character from input

Characters are internally stored as an ASCII value ('A' stored as 65)

Use escape sequences to store certain characters

## Strings

String! a sequence of characters, surrounded by double quotes

String variables refer to string objects by reference

.next() skips whitespace in a string and stops at whitespace
.nextLine() gets all remaining text on current line, up to the next newline (which is removed but not put into the variable)

## Integer Overflow

Overflow: value being assigned to a variable is greater than the maximum value that variable can store
(~2 billion for an int)

If too much Math is going to cause an int to overflow, use a long instead

## Numeric Data Types

In ascending order of storage space:
* byte
* short
* int
* long

Same but with floating point data types:
* float
* double

## Random Numbers

Random class can generate a wide range of random integers

import java.util.Random
Random randGen = new Random();
randGen.nextInt(n);

Providing an argument limits the random values to 0 and n-1

Can also create a pseudo-random class using a seed (value passed to new Random();)