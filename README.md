# EXP-2
# Harshil Nagori
# EnTC A2
# 24070123046
Aim

To:

    Understand and use data types in C++

    Explore storage classes – auto, static, extern, register

    Learn about variable scope and how many bytes are allocated to each data type

Objectives

🔹 Apply different storage classes 🔹 Understand the storage, scope, and default values of each class 🔹 Learn how to check the memory size of data types using sizeof
Program Overview
Syntax of the program

We create a user-defined function to see how variables behave under different storage classes.

The main() function calls that user-defined function.

We use the sizeof operator to find how many bytes are used by each data type.
Auto Storage Class

Auto is the default storage class for all local variables.

These variables exist inside functions and get deleted when function ends.

Their default value is undefined (garbage).

auto int x;

Extern Storage Class

Used to refer to a global variable declared outside the function.

extern tells the compiler the variable exists somewhere else (cannot initialize it here).

Its default value is garbage.

extern int x;

Static Storage Class

Keeps the variable alive through all function calls – it doesn’t reset.

Used mostly in functions to preserve previous values.

Default value is zero (0).

static int x;

Register Storage Class

Tells compiler to store the variable in a CPU register (for faster access).

You can’t use &x with register variables because they don’t have a memory address.

Default value is garbage.

register int x;

What I Used

Storage Classes: auto, extern, static, register

Data Types: int, float, char, bool, short, long, double

sizeof operator to check data type sizes
Sample Output
Auto Storage Class

Size of variable: 4
The variable is :6

Address of func variable a: 0x7ffccd69c61c
Size of variable: 4
The variable is :6

Address of func variable a: 0x7ffccd69c61c
Size of variable: 4
The variable is :6

The variable is :7
Address of global variable a: 0x404040

Static Storage Class

Address of func variable a: 0x404194
Size of variable: 4
The variable is :1

Address of func variable a: 0x404194
Size of variable: 4
The variable is :2

Address of func variable a: 0x404194
Size of variable: 4
The variable is :3

The variable is :5
Address of global variable a: 0x404040

Register Storage Class

Size of variable: 4
The variable is :-1170925895

Size of variable: 4
The variable is :-1170925895

Size of variable: 4
The variable is :-1170925895

The variable is :4
Address of global variable a: 0x404040

Extern Stoareg Class

Address of func variable a: 0x404040
Size of variable: 4
The variable is :4

Address of func variable a: 0x404040
Size of variable: 4
The variable is :5

Address of func variable a: 0x404040
Size of variable: 4
The variable is :6

The variable is :6
Address of global variable a: 0x404040

Size of datatype

Size of various datatypes
Integer: 4
Float: 4
Boolean: 1
Long Integer: 8
Short Integer: 2
Double: 8
Character: 1
