# Printf

This is a custom implementation of the standard C library function `printf()` using the C programming language. It is a simplified version of the original `printf()` function, which allows users to print formatted strings to the console.

## Getting Started

### Prerequisites

To use this implementation of `printf()`, you will need:

* A C compiler (such as GCC)
* A Unix-like operating system (such as Linux or macOS)

### Installing

To use `printf()`, simply download the `printf.c` file and include it in your project. You can then use the `printf()` function in your code.

## Usage

The `printf()` function works by taking a string as its first argument, which may contain special format specifiers that start with `%`. For example, `%d` is used to format an integer value, and `%s` is used to format a string.

Here's an example of how to use `printf()` to print a formatted string:

```c
#include "printf.h"

int main() {
    int my_number = 42;
    printf("My favorite number is %d!\n", my_number);
    return 0;
}

When you run this program, it will print the following output:

> My favorite number is 42!

## Supported Format Specifiers

This implementation of `printf()` supports the following format specifiers:

- `%c` - format a character value
- `%d` - format an integer value
- `%s` - format a string value
- `%x` - format an unsigned hexadecimal integer value
- `%u` - format an unsigned integer value

To use a format specifier, include it in the format string passed as the first argument to `printf()`. For example:

```c
#include "printf.h"

int main() {
    char my_char = 'X';
    int my_int = 42;
    unsigned int my_unsigned_int = 123;
    char* my_string = "hello, world!";
    
    printf("my_char: %c\n", my_char);
    printf("my_int: %d\n", my_int);
    printf("my_unsigned_int: %u\n", my_unsigned_int);
    printf("my_string: %s\n", my_string);
    
    return 0;
}

This program will print the following output:

my_char: X
my_int: 42
my_unsigned_int: 123
my_string: hello, world!
