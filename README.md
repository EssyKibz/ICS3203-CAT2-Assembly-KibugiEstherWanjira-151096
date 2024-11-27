# ICS3203-CAT2-Assembly-KibugiEstherWanjira-151096

# Assembly Projects

This repository contains several assembly language programs written in NASM (Netwide Assembler). Each program demonstrates different aspects of low-level programming, including user input handling, arithmetic operations, conditional jumps, and hardware simulation.

## Table of Contents

- [Introduction](#introduction)
- [Programs](#programs)
  - [Positive/Negative/Zero Identification](#positivenegativezero-identification)
  - [Automation Control](#automation-control)
  - [Factorial Calculation](#factorial-calculation)
  - [Array Reversal](#array-reversal)
- [Requirements](#requirements)
- [Running the Programs](#running-the-programs)
  - [Positive/Negative/Zero Identification](#running-positive-negative-zero-identification)
  - [Automation Control](#running-automation-control)
  - [Factorial Calculation](#running-factorial-calculation)
  - [Array Reversal](#running-array-reversal)
- [Challenges](#challenges)


## Introduction

This repository includes various assembly language programs, each focusing on different concepts and functionalities. The programs are intended for educational purposes to understand low-level programming and assembly language concepts.

## Programs

### Positive/Negative/Zero Identification

This program prompts the user to enter a number and then identifies whether the number is positive, negative, or zero.

### Automation Control

This program simulates a simple automation control system where a sensor value is read, and based on the value, it controls a motor and an alarm.

### Factorial Calculation

This program prompts the user to enter a number between 1 and 10 and then calculates the factorial of that number using a recursive function.

### Array Reversal

This program prompts the user to enter 5 integers, stores them in an array, and then reverses the array in place without using additional memory.

## Requirements

- NASM (Netwide Assembler)
- Linux environment (for syscall usage)

## Running the Programs

### Running Positive/Negative/Zero Identification
   ```sh
   nasm -f elf64 -o data_monitoring.o data_monitoring.asm
   ```
   ```sh
   ld -o data_monitoring data_monitoring.o
   ```
   ```sh
   ./data_monitoring
   ```

### Running Automation Control
   ```sh
   nasm -f elf64 -o controlflow.o controlflow.asm
   ```
   ```sh
   ld -o controlflow controlflow.o
   ```
   ```sh
   ./controlflow
   ```

### Running Factorial Calculation
   ```sh
   nasm -f elf64 -o factorial.o factorial.asm
   ```
   ```sh
   ld -o factorial factorial.o
   ```
   ```sh
   ./factorial
   ```

### Running Array Reversal
   ```sh
   nasm -f elf64 -o array.o array.asm
   ```
   ```sh
   ld -o array array.o
   ```
   ```sh
   ./array
   ```

## Challenges

While running the programs, you may encounter the following challenges:

1. **Floating Point Exception (Core Dumped)**: This error can occur if there is a division by zero or if the stack is not properly managed in programs like the factorial calculation.
2. **Input Handling**: Ensure that the input values are within the expected range to avoid unexpected behavior.
3. **Assembly Syntax Errors**: Double-check the NASM syntax and ensure all instructions and directives are correctly used.
4. **Linking Issues**: Ensure that the object files are correctly linked. Any missing dependencies or incorrect linking commands can lead to executable errors.



