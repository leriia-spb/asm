# Asm-task

## Task
This repository contains assembly programs:

* `add.asm` — a program that performs addition of two long numbers.
* `sub.asm` — a program that performs subtraction of two long numbers.
* `mul.asm` — a program that performs multiplication of two long numbers.

# Overview

To run the program, you will need any 64-bit Linux distribution.

## Build Instructions

All actions in the instructions are performed from the root of the repository.

#
```console
$ sudo apt install binutils g++ cmake nasm
$ ./build.sh
```

### Running an Example
```console
$ ./build/add
10000000000000000000000000000000000000
100000000000000000000000000000000000000000000000000000000000000
100000000000000000000000010000000000000000000000000000000000000
```

## Notes
1. The mul and sub operations work with unsigned numbers of a maximum length of 128 qwords (input). At the same time, the result of mul (output) can be up to 256 qwords long, and this is handled correctly.
2. In the sub operation, the minuend is always greater than or equal to the subtrahend.







