# Objects

Objects: internal data items plus operations that can be performed on that data

Class: defines the data and operations that go with an object

Variable: named item used to hold a value

Variable declarations specifies a variable's name and type; assigns that variable to a memory location
Assignment statements give the variable a value

Identifiers rules

Use camelCase or under_score to separate words in an identifier

An expression evaluates to a value, which replaces the expression

Incremental development: writing, compliling, and testing small amounts of code at a time; adding as you go

Integer types: typically used for values that are counted (can only be whole numbers)
Float types: best for measurements, or fractions of countable items (averages)

NaN (not a number): unrepresentable or undefined values

Dividing by 0.0 results in "infinity"

0.0 / 0.0 = NaN

Printf!
Decimal precision

Comments

Whitespace: mostly ignored by the compiler, but makes the program easier to read by other humans

Method call- invokes an object's methods, usually object.method(arguments)

Public methods: can be invoked directly on objects of a class; class interface; methods are listed after the "public" keyword

Private methods: internal data, listed after the "private" keyword

*Parameters* are the input specified in the method definition, *arguments* are the values passed to a parameter

Methods can return one value or none, methods that do not return a value are specified **void** in the method declaration

Constructing objects involves:
* Creating a reference variable (refers to the object)
* *new* operator: keyword *new* creates a new variable
* Constructor to initialize interal data

Histogram marblesHistogram = new Histogram();

Classes can define multiple constructors with different parameter types

Mutator methods modify object data, accessors show object data

Module: group of related packages
Package: group of related classes

Graphical application: displays drawings and other graphical objects