# Methods and Classes

Class construct defines a new type that can group data and methods to form an object
Public member methods: operations a user can perform on the object

User does not need to know how the data and methods are implemented, jsut how each public method behaves

Reference variable refers to an instance of the class, *new* operator creates an object of the specified class type

Private fields: variables that member methods can access, but class users cannot

to define a class:
1. name the class
2. declare private fields
3. define public member methods

main() is independent of class objects, can access other static methods and fields of the object, but not non-static methods or fields
Create objects within main() to call non-static methods

Method: named list of statements
Method definition: method's name and block of statements to execute
Method call: invocation of the method, causing it execute

main() indicates the start of a program

Methods can return values (instead of printing them), type of return value must be specified at beginning of the method; can return one or less values

Methods can call other methods

Using defined methods makes main() easier to read

Modular development: dividing a program into separate modules that can be tested and then integrated
Incremental development: programmer develops small pieces of the program at a time, tests, and moves on
Method stub: method definitions whose cade hasn't been written- useful for determining behavior of main() and required methods

Code should not be redundant, if you use the same code in the program more than once it may be better suited to a method

**Unit testing!**

Uses a testbench program to test a program through a series of input/output checks

Should perform automatic checks, go through every line of code, uses new values each time, and checks border cases (unusual or extreme values)

Regression testing: retesting an item after the item is changed

**this**

implicit parameter: object reference before a method name (ex *Math*.pow())

Within a member method, an implicit parameter can be replaced by *this*

