Libft Tester

A simple test suite for the 42 School libft project.

It tests mandatory and bonus functions to help identify bugs and verify your implementations.

Compilation

Compile the tester with your libft source files:

bash
gcc -Wall -Wextra -Werror test.c *.c -o test


If *.c includes test.c, exclude it to avoid duplicate main() errors:

bash
gcc -Wall -Wextra -Werror test.c $(ls *.c | grep -v '^test.c$') -o test

Usage

Run all tests:

bash
./test all


Run a specific test:

bash
./test strlen
./test split
./test lstmap


Display available tests:

bash
./test

Features
Tests mandatory libft functions.
Tests bonus linked-list functions.
Displays passed and failed checks.
Allows running individual tests.
Uses temporary files to test file descriptor functions.
Disclaimer

This is an unofficial tester. Passing all tests does not guarantee a perfect evaluation at 42.
