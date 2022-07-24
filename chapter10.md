# Chapter 10: Inheritance

One class can be derived from another
Derived class (subclass) inherits properties of base class (superclass)
*extends* derives one class from another
One base class can be used for multiple derived classes

Classes of a derived class have access to public members of base class

protected: derived classes and other classes in package have access

private: accessible by self
public: accessible by self, derived classes, everyone
protected: accessible by self, derived classes, classes in same package
none given: access by self and other classes in package

Overriding: derived class member method that has the same name and parameters as a method in the base class
@Override specifies that an identical base class method exists
Derived class method takes precedence over base class method

Can still call a base class method using super.methodName()

Object class: base class for all other classes, including user-made classes
.toString() returns a string representation of the object
.equals(otherObject) returns true if both variables reference the same object

Polymorphism: determining which behavior to execute based on data types
Compile-time polymorphism: compiler determines which method to run based on parameter types; overloading
Runtime polymorphism: determination is made while program is running

Reference to derived class can be converted to a reference to the base class

Abstract classes: cannot be instantiated, may guide the design of subclasses

Abstract method: not implemented in base class, all subclasses must override
Concrete class: not abstract

Composition: one object may be made up of other objects

UML: used to model the classes in a program
Consists of:
Class name
member variable name and type
method name and return type
- for private, + for public

Uses arrows to indicate relationships; solid arrow points towards the superclass
Italics for abstract classes
Dashed line points to interface

Interface: set of abstract classes that an implementing class must override and define