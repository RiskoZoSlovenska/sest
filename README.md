# sest

`sest` (a contraction of "simple" and "test") is a simple utility script which reads test cases from a file, then runs a target script with appropriate input and compares the expected and actual output.

Focus is on ease-of-use. Some features include:
* Automatically run multiple tests
* All tests are stored in the same file
* Zero configuration required
* Dead-simple syntax
* Coloured and controllable output

Currently only Python is supported, but PRs are more than welcome!


# Motivation 

I occasionally participate in programming competitions where you write a small script to read some input from stdin, and then print the answer to stdout. If you ever want to test the program before submitting it for evaluation, you have to run it through terminal, copy-paste the input and then compare the output with the expected output.

This is, of course, tedious and prone to human error, especially when you have multiple test cases. One option is to write all the test case inputs into files and then redirect stdin to read from those files, but this way you still have to run all the cases individually and can't check for invisible errors (such as trailing spaces).

Thus, `sest` was born.


# Installation

The only dependency is a non-ancient Bash.

Just clone/download the repo/file and then copy/move/link the file to your `bin` folder.