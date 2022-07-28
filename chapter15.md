# Chapter 15: Input/Output

Output stream: class that supports output (OutputStream)
provides methods for writing bytes to a destination

InputStream: for receiving input

System.in and System.out are predefined, do not need to import

Byte stream returns value of -1 if there is no more data to read

throws IOException: throws clause for when program may quit unexpectedly due to an exception (error reading from an input stream)

flush() flushes buffer contents
System.out.flush() writes contents of buffer to screen
Flush also happens when newline character or println is used

input string stream: scanner object initialized from a string
output string stream: same, but for output (needs StringWriter and PrintWriter)

## Output Formatting

printf() and format() for adjusting the appearance of output

format specifiers:
%c - char
%d - int, long, short (decimal)
%o - int, long, short (octal)
%h - int, long, short, char (hex)
%f - float, double
%e - float, double (scientific)
%s - string
%% - % character
%n - newline character

### Sub Specifiers

%(flags)(width)(.precision)specifier

width: minimum characters to print, padded if value is shorter

flags:
-: left aligns output
+: prints plus for positive values
0: pads output with 0s
space: space for positive values

(floats)
precision: digits after decimal point, 6 by default

## Files

Files can be used for input/output, instead of screen

input: create a FileInputStream object, using name of file as an argument
Read file until end using a loop
hasNextInt() (and similar methods) return true if there is another int available

FileOutputStream() uses filename as an argument, writes to that file
1. open the file
2. create a printwriter to write to the file
3. print to the file
4. close the file!