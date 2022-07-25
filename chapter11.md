# Chapter 11: Generics

Java's Collections class provides static methods useful for completing common tasks 

Wrapper classes implement the Comparable interface, which includes the .compareTo() method

You can use .sort() on an ArrayList of a type that implements the Comparable interface

import java.util.Collections

.sort() can also sort an ArrayList of a user-defined type; user-defined class must also implement Comparable and override the compareTo() method
compareTo should return a number (-1, 0, 1) that determines the order of the two objects

use the *implements* keyword to show that a class implements an interface

interfaces cannot be instantiated, methods must be overridden by the implementing classes

### Generic Methods

Instead of writing similar methods that vary only by data type...

use a generic method!

<TheType extends Comparable<TheType>> in the method header
indicates a template parameter that can be used for any data type

Type bounds specify valid class types for a parameter, specified after *extends*
ex: extends Comparable means data types are bound to types that implement Comparable

### Class Generics

Same idea as above, but with classes

Generic class: class definition with a special type parameter that may be used in place of types in the class
<TheType ...> is the type parameter and can be used throughout the class

Type arguments must be reference types, not primitive types

????????