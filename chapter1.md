# Chapter 1

## 1.2 Input/Output

Input

Programs commonly get input, perform magic, and produce output

Scanner (java.util.Scanner): text parser that can get input from a source. Create a scanner object

Output

System.out.print() prints output, multiple print commands printed to the same line
System.out.println() starts a new line after the output

Can print a string literal (with " ") or a variable value

## 1.3 Errors

Syntax errors: violates the rules of the language

Compilers may point to an error in a line *after* the error actually occurs. Error could be different than what the compiler states (missing parentheses instead of semicolon)

Focus on fixing the first error

Successful compiling means the program doesn't have any compile-time errors (syntax errors), but could still have logic errors

Logic error: program compiles, but doesn't run as intended

Compiler warning: doesn't stop the compiler from working, but may indicate a logic error