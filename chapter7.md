# Chapter 7: Arrays

Variable for storing a list of data items

Element: each item in an array

Index: location of an element in the array (starts at 0)

In Java:
datatype[] arrayName = new datatype[length]
Can declare and allocate separately, but best to do both at the same time

Arrays are reference variables

Array elements are automatically initialized to default values when using the *new* keyword
You can initialize non-default values by:
dataType[] arrayName = {value, value, value...}

Use loops to iterate through arrays and read each value individually; you can use this to determine the max value in a list

If checking for the min or max, initialize the holding variable to the first value in the array!

To swap two elements in an array, you will need to use a temp variable to hold one of the values
If you copy the first value to the next index, the value at the next index is now gone

tempVal = x;
x = y;
y = tempVal;

You can also modify/copy arrays while iterating

## Two-Dimensional Arrays

Arrays can be initialized with two dimensions:
int[][] myArray = new int[R][C]

Rows, columns

2D arrays are really just an array of arrays
R = number of arrays
C = elements in each array

Can initialize table with non-default values using braces

## For each loop

Iterates through an array, declares a new loop variable

for (dataType loopVariable : arrayName) {
    do an action for each element in the array
}

loopVariable is the variable name for the current element in the iteration