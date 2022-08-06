# Chapter 16: Exceptions

Exception: unexpected incident that stops the normal execution of a program

Try/catch blocks handle exceptions during the program
Try: surrounds normal code, exited immediately if there is an exception
Catch: "catches" exceptions, code within the block executes if an exception matches the block's parameter type

Programs can exit code if an exception occurs, or attempt (to get data) again

Throw: throws a throwable object during execution; creates and throws an exception

Code within a try block can throw different types of exceptions

try-with-resources: declares closable resources (like files)

finally: executes when the try block exits

throws clause: specifies types of exceptions a method may throw; may specify multiple exception types

Checked exception: programmer should be able to anticipate and handle (filenotfound exception for program that deals with files)
Unchecked exception: caused by hardware or logic errors

Checked methods are required to be caught using a catch block, or specify a thrown exception using a throws clause