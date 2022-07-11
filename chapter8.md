# Chapter 8: Methods

Methods may include branches, loops, and other statements. 

Unit testing: individually testing a small part of the program, usually done using a testbench or test harness (separate program designed to test that methods return the expected values)
Test vector: set of input values for testing

Assert: prints an error message and exits the program if the provided test expression evaluates to false
assert testExpression : detailedMessage

Test vectors should throroughly check the method for many different cases, including border cases (extreme values)

Each method call creates a new set of local variables; return causes those variables to be discarded

Primitive variables are passed by value to a method- the actual value is copied into a local variable for use
Arrays are passed by reference- the method can modify the contents of the array

Scope: variables declared in a method are valid from the variable declaration to the method's closing brackets

Variable declared within a class (but outside a method) is valid from the beginning of the class to the end

Method scope: from class opening brace to closing brace

Overloading: giving multiple methods the same name but different parameters
Parameters must be different types
Return type does not affect overloading

Good practice to check parameter values and assign a default value to parameters outside the expected values

Only use one input Scanner per stream
Create one Scanner object in main() and pass that to methods as needed

Documentation: description of the program and its components

Javadoc parses specifically formatted multi-line comments and generates documentation in HTML format

Block tags:
@author
@version
@param: describes a parameter and its purpose
@return: describes return type and purpose
@see: refers to relevant information