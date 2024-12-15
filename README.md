# Dereferencing a Null Pointer in C++

This repository demonstrates a common C++ error: dereferencing a null pointer.  Dereferencing a null pointer (attempting to access the memory location pointed to by a null pointer) leads to undefined behavior, most often resulting in a segmentation fault (crash) of the program.  This example shows how to avoid this error.

## The Bug (`bug.cpp`)

The `bug.cpp` file contains the faulty code that causes the problem.  It attempts to assign a value to memory that the pointer `ptr` is not pointing to anything. 

## The Solution (`bugSolution.cpp`)

The `bugSolution.cpp` file demonstrates the corrected code. Before dereferencing `ptr`, it checks if `ptr` is null using an `if` statement.  If it's null, an error message is printed; otherwise, the value assignment proceeds safely.