Tasks
0. isupper
mandatory

Write a function that checks for uppercase character.

    Prototype: int _isupper(int c);
    Returns 1 if c is uppercase
    Returns 0 otherwise

FYI: The standard library provides a similar function: isupper. Run man isupper to learn more.

julien@ubuntu:~/0x04$ cat 0-main.c
#include "main.h"
#include <stdio.h>

/**
 * main - check the code.
 *
 * Return: Always 0.
 */
int main(void)
{
    char c;

    c = 'A';
    printf("%c: %d\n", c, _isupper(c));
    c = 'a';
    printf("%c: %d\n", c, _isupper(c));
    return (0);
}
julien@ubuntu:~/0x04$ gcc -Wall -pedantic -Werror -Wextra -std=gnu89 0-main.c 0-isupper.c -o 0-isuper
julien@ubuntu:~/0x04$ ./0-isuper 
A: 1
a: 0
julien@ubuntu:~/0x04$ 

Repo:

    GitHub repository: alx-low_level_programming
    Directory: 0x04-more_functions_nested_loops
    File: 0-isupper.c


1. isdigit
mandatory

Write a function that checks for a digit (0 through 9).

    Prototype: int _isdigit(int c);
    Returns 1 if c is a digit
    Returns 0 otherwise

FYI: The standard library provides a similar function: isdigit. Run man isdigit to learn more.

julien@ubuntu:~/0x04$ cat 1-main.c 
#include "main.h"
#include <stdio.h>

/**
 * main - check the code
 *
 * Return: Always 0.
 */
int main(void)
{
    char c;

    c = '0';
    printf("%c: %d\n", c, _isdigit(c));
    c = 'a';
    printf("%c: %d\n", c, _isdigit(c));
    return (0);
}
julien@ubuntu:~/0x04$ gcc -Wall -pedantic -Werror -Wextra -std=gnu89 1-main.c 1-isdigit.c -o 1-isdigit
julien@ubuntu:~/0x04$ ./1-isdigit 
0: 1
a: 0
julien@ubuntu:~/0x04$ 

Repo:

    GitHub repository: alx-low_level_programming
    Directory: 0x04-more_functions_nested_loops
    File: 1-isdigit.c

