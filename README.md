Overview
This repository contains the implementation of a custom printf function in C as part of the SE Foundations curriculum. The project replicates the behavior of the standard C library printf function, covering various format specifiers and custom features.

Project Requirements
Programming Language: C
Compilation: Ubuntu 20.04 LTS using gcc
Code Style: Betty style
Editors: vi, vim, emacs
No. of Functions per File: Maximum of 5
Header File: main.h
Global Variables: Not allowed
Main Function: Not to be pushed to the repository root
Allowed Functions and Macros
write
malloc
free
va_start
va_end
va_copy
va_arg
Compilation Instructions
To compile the code:

bash
Copy code
gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c
Ensure no C files containing main are pushed to the root directory.

Features and Specifiers Implemented
Basic Format Specifiers:
%c: Character
%s: String
%%: Percent sign
Integer Specifiers:
%d, %i: Signed decimal integer
Custom Format Specifiers:
%b: Binary
%u: Unsigned decimal integer
%o: Octal
%x, %X: Hexadecimal (lowercase and uppercase)
%S: String with non-printable characters as \x followed by ASCII value
%r: Reversed string
%R: ROT13 encoding
Advanced Features:
Buffer management to minimize write calls
Flag characters: +, space, #
Length modifiers: l, h
Custom handling for non-printable characters
Usage Example
c
Copy code
#include "main.h"

int main(void)
{
    _printf("Let's try to printf a simple sentence.\n");
    _printf("Character:[%c]\n", 'H');
    _printf("String:[%s]\n", "I am a string !");
    _printf("Unsigned:[%u]\n", 2147484671);
    _printf("Unsigned octal:[%o]\n", 2147484671);
    _printf("Unsigned hexadecimal:[%x, %X]\n", 2147484671, 2147484671);
    _printf("Binary:[%b]\n", 98);
    _printf("Reversed:[%r]\n", "Hello");
    _printf("ROT13:[%R]\n", "Hello");
    return (0);
}
Contributing
This project was completed as a group effort. Only one project repository should exist per group to avoid the risk of scoring 0%.

License
This project is licensed under the terms of the ALX program and is protected by plagiarism policies. Any form of content reproduction or publishing is prohibited.

Author
This project was developed by a team as part of the SE Foundations curriculum under the ALX program.
