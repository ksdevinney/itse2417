# Lööps

Loops repeatedly execute the body statements while the loop's expression is true

Loops can examine a list of values, one at a time

## While Loops

Repeatedly executes the loop body while the entry condition evaluates to true
Often uses a relational operator to evaluate entry condition

Sentinel value: indicates the end of a list; controls program stop

## For Loops

Loops that must execute a determined number of times

At the top, requires:
* loop variable initialization
* loop expression
* loop variable update

++ increment operator
-- decrement operator
Both of the above can go before or after the variable; ++i increments before evaluating, i++ increments after

When to use **for** vs **while**?
For: number of iterations is computable before the loop
While: not easy (or possible) to determine how many iterations are required

Generally, for loops:
* initialize loop variable with 0 instead of 1
* use < instead of => when checking condition
* loop variable can be declared inside or outside of the loop

Loops can be used to inspect a string, one character at a time

Nested loops occur in the body of another loop; can be used to generate all combinations of items

## Break and Continue

Break statements cause an immediate exit from the loop

Continue statement: immediately jumps to the loop condition check

Both can improve readability, but may not be necessary

## Scope

Region of code where a declared variable is valid

Variables declared in a block of code (between curly bois {}) are only valid until the closing brace

## Enumerations

Custom variable type

enum declares a name for the new type and all possible values

public enum identifier {enumerator 1, enumerator 2...}

enumerators are named constants

Must include identifier when declaring variables of that type:
Identifier testVariable = Identifier.VALUE;

Enumerations may be less prone to error, require less code than finals and strings