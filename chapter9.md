# Chapter 9: Classes Continued

Class public methods are either mutators (modify a class's fields) or accessors (accesses/returns fields)

Setters: set a field value
Getters: get the field value

Private helper methods help public methods carry out tasks

You can initialize field variables in their declaration; objects created will automatically have those values

Constructors: used to initialize fields of an object
If there is no defined constructor, Java automatically initlizes all field variables to default values
You can *overload* constructors by creating multiple constructors with different parameter types
Good practice to define a no-argument constructor

Reference variables refer to an object; store the memory of the object instead of the value
More than one reference variable can refer to the same object

Abstract Data Types: uses information hiding; user only needs to know interface and not implementation

## Primitive and Reference Types

Wrapper classes: built-in reference types that augment primitive data types
Provide methods for converting between data types
Create reference variables
Wrapper class objects are immutable; new memory allocation occurs every time a new value is assigned

comparison operators (== and !=) for wrapper class objects actually compare memory location
Can use comparison for wrapper objects to primitive variables and literals
Somehow < => <= > are okay?
Otherwise use ReferenceVar1.equals(ReferenceVar2) and .compareTo 

Autoboxing: automatic conversion of primitive types to wrapper class variables
Unboxing: conversion of wrapper class variables to primitive data types

Also methods for converting wrapper class variables to primitive types

ArrayList: ordered list of reference type items
Can grow and shrink to fit number of elements
.add()
.get()
.set()
.size()

Collection: generic group of elements

Using a reference variable as a parameter assigns the stored reference as the parameter

## Static Fields and Methods

Static: variable only allocated once in memory during program execution
Static fields: fields of the class; independent of objects and can be accessed without creating a class object
Class variables (non-static fields are instance variables)

Static member method: method independent of class objects
Can only access a class's static fields