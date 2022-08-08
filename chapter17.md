# Chapter 17: Recursion

Recursive algorithm: breaks the problem into smaller problems and applies the same algorithm to solve smaller problems

Recursive methods create a new "copy" of themselves as they attempt to reach the base case

Binary search works with recursion

Increasing indents can be helpful for debugging

Creating a recursive method:
* write the base case (value returned without performing recursion)
* write the recursive case

binary search:
* base case: number is found
* recursion: item is larger than midpoint (binary search on upper half)
* recursion: item is lower than midpoint (binary search on lower half)

More than one base case can exist

Common errors:
* not covering all base cases
* recursion never reaches base case

Recursive math: Fibonacci sequence, greatest common divisor

Recursion can provide all possibilities for a situation

Stack overflow: stack frame extends beyond memory allocated for a stack
Each method call uses a new stack frame; frames are deleted upon return