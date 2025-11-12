HERE I WILL DEMONSTRATE MY CODE

"Aliquot Sequence Calculator"
OVERVIEW:
aliquot.c is a C program that computes aliquot sequences for a given starting number. An aliquot sequence is a sequence of numbers in which each term is the sum of the proper divisors of the previous term. Proper divisors of a number are all its positive divisors excluding the number itself.

The program allows you to either print the full sequence or just find the length of the sequence, and supports large numbers up to 10^15


 It has two display modes:

- Full sequence (f) – prints every term of the sequence.

- Length only (l) – prints only the length of the sequence.

(Optional limit on sequence length to prevent infinite loops.)

Handles edge cases for numbers 0 and 1.

COMPILATION:

To compile the program, use a standard C compiler such as gcc:

gcc -O0 -m32 -Wall -Wextra -Werror -pedantic -o aliquot aliquot.c

This will generate an executable named aliquot.

USAGE:

Run the program and follow the prompts:

./aliquot


The program will ask for:

Starting number: Enter a positive integer less than 10^15


Maximum sequence length: Enter 0 for no limit, or a positive integer to limit the number of terms.

Display mode: Enter 'f' to print the full sequence or 'l' to print only the length.

EXAMPLES:

Example 1: Full sequence
Please, give the number to start the aliquot sequence from: 12
Provide the max aliquot length to look for (0 for unlimited): 0
Do you want to print the full sequence ('f') or just the length ('l')? f
12
16
15
9
4
3
1
0


Example 2: Length only
Please, give the number to start the aliquot sequence from: 12
Provide the max aliquot length to look for (0 for unlimited): 0
Do you want to print the full sequence ('f') or just the length ('l')? l
Length of the aliquot sequence: 8

Notes

If a number in the sequence exceeds 10^15, , the program will stop and display an error.


The sequence stops when it reaches 0 or stabilizes (i.e., when a term repeats itself e.g. the number 6).

Proper input validation is implemented to prevent invalid or negative numbers.
