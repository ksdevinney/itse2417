# Chapter 5: Branches

Branch: sequence of statements executed only under certain conditions

If-else: *if* branch is executed if a condition is true, otherwise the *else* branch is executed

If-elseif-else: each branch is checked in sequence, if one branch's condition is true that branch is taken; *else* is taken if no branch is true

== equality operator
!= inequality operator

Floating point values should not be compared using equality operators

Comparing characters compares their unicode numbering

Logical operators:
a && b: both conditions must be true
a || b: either condition can be true
!a: true if a is false

To detect a range of values:
x must be larger than the lower end, AND smaller than the upper end

Can explicitly declare a range (using &&), or implicitly: checking if value is greater than certain intervals

You can use multiple distinct *if* statements to check many non-mutually exclusive categories

Precedence rules:
()
!
* / % + - (still following their precedence rules)
< <= => >
== !=
&&
||

Switch statements: can be used to detect multi-branch behavior for specific expected values (only char, string, or int)
Include a case for each expected value, with a default behavior at the end
break statements allow you to exit the branch, breaks can be intentionally left out if several conditions have the same outcome

Boolean: data type, can only be true or false

To compare strings, use .equals()- compares two strings, returns true if they are equal
Strings are compared relationally, using unicode values (captical letters < lowercase letters)
String1.compareTo(string2) returns:
-1 if string 1 is less
0 if both strings are equal
1 if string 1 is greater

String indexes start with 0

charAt(x) returns the character at index x
.length() returns the total length of a string, the last character is located at length - 1

.isLetter(), .isDigit(), .isWhitespace() return true or false
.toUpperCase() and .toLowerCase() convert the string if possible, nothing happens if not possible (numbers, special characters)

.indexOf(item, index) returns the first index of x; optionally starting at index
.substring(startIndex, endIndex) returns a substring starting at startIndex and (optionally) ending at endIndex - 1

.concat(newString) adds newString to the end of the first string
.replace(findStr, replaceStr) replaces all instances of findStr with replaceStr
Strings are immutable- all above methods should be assigned to a variable, original string will not be changed

Conditional expression:
x = (y > 0) ? 6 : 3;
checks condition before ?, assigns first value if true and second value if not
Can replace an if/else

## Floating Point comparison

Do not use == to compare floating point values- floats may not be exactly represented; they may be close but not exactly equal

Instead, use Math.abs(x - y) < 0.0001
The difference between float (or double) variables x and y should be less than 0.0001 for them to be considered "close enough"

Epsilon: difference threshold indicating two numbers are close enough to be equal; often 0.0001 but not always

Short circuit evaluation: skips evaluating later operands if the result of a logical operator can already be determined (if one operand of && is false, the whole thing is false; if one operand of || is true, the whole thing is true)