# C-Seminar-labs---Tu-Sofia
My experience  with C program language through second half of the first eyer in Technical University - Sofia.

This repository contains a systematic collection of C programming source codes developed during university laboratory sessions in the second semester at the Technical University of Sofia. The projects cover core computer science concepts, structured programming, memory management, and modular software design using header files.

---

## 📌 Contents by Laboratory Exercise

### 📂 Lab 1: Basic Syntax, Data Types & Operators
* **`lab1zad1.c`**: Input/output operations with different formatting specifiers (`%d`, `%f`, `%c`), octal/hexadecimal conversions, and exploring memory sizes using `sizeof`.
* **`lab1zad2.c`**: Basic arithmetic operations and type casting experiments between integer and real numbers.
* **`lab1zad3.c`**: Floating-point precision analysis, comparing `float` and `double` representations up to 17 decimal places.
* **`lab1zad4.c`**: Detailed demonstration of prefix and postfix increment (`++`) and decrement (`--`) operators.

### 📂 Lab 2: Control Flow & Loops
* **`lab2zad1.c`**: Factorial calculation using `for` loops, handling corner cases like $0!$.
* **`lab2zad2.c`**: Simple interactive calculator implemented via a `switch-case` structure, including input buffer management.
* **`lab2zad2b.c`**: Quadratic equation solver ($ax^2 + bx + c = 0$) handling real, equal, and complex roots via `<math.h>`.
* **`lab2zad4.c`**: Loop control structure with data validation, using `continue` to filter and sum only even numbers.

### 📂 Lab 3: Functions & Pointers
* **`lab3zad1.c`**: Comparison between passing arguments **by value** versus **by reference** (using pointers).
* **`lab3zad2.c`**: Generating the Fibonacci sequence up to a user-defined limit using a standalone function.
* **`lab3zad3.c`**: Advanced usage of **function pointers** (`int (*fp)(int, int)`) to build an interactive menu-driven math application.

### 📂 Lab 4: Arrays & Sorting Algorithms
* **`lab4zad1.c`**: Implementation of the **Selection Sort** algorithm to arrange an integer array in ascending order.
* **`lab4zad2.c`**: Implementation of the **Quick Sort** (divide and conquer) algorithm using recursion, boundaries (`left`, `right`), and a central pivot.

### 📂 Lab 5: String Manipulation
* **`lab5zad1a.c`**: Manual string length extraction using a bodyless `for` loop, tracking the null-terminator (`\0`).
* **`lab5zad2.c`**: String sorting program utilizing a custom 2D `char` array, sorting 5 words alphabetically using `strcmp`, `strcpy`, and `strlen`.
* **`lab5zad11b.c`**: Manual string concatenation logic (recreating standard `strcat` functionality).
* **`lab5zad11c.c`**: Manual string copying logic (recreating standard `strcpy` functionality).

### 📂 Lab 6: User-Defined Data Structures (Structures)
* **`lab6zad1.c`**: Working with `struct BOOKS`. Demonstrates passing structures to functions by value for data printing and dynamic record creation.
* **`lab6zad2.c`**: Implementing an array of structures (`struct Books library[5]`) to manage books systematically via indexed structural memory.

### 📂 Lab 7: File Handling & Multi-File Modular Design
This lab demonstrates proper enterprise-level architecture by separating code into **Main entry points**, **Function definitions**, and **Header files (`.h`)**.

#### 📝 Project 1: Text File Processing & Analysis
* **`lab7zad1main.c`**: The central interactive text-based menu.
* **`lab7zad1menu.c` & `lab7zad1menu.h`**: Modular menu parsing component.
* **`lab7zad1header.h`**: Centralized inclusion of system libraries and internal headers.
* **`lab7zad1.h`**: Declares advanced text file processing capabilities:
    * Finding minimum and maximum values within a text file.
    * Filtering data points belonging to a specific interval.
    * Calculating arithmetic averages and replacing negative values inside the text stream.

#### 📝 Project 2: Binary File Processing with Geometric Structures
* **`lab7zad2main.c`**: Main driver for custom binary storage operations.
* **`lab7zad2header.h`**: Defines a geometric coordinate structure using a `typedef struct`:
    ```c
    typedef struct {
        int x;
        int y;
    } Point;
    ```
* **`lab7zad2funcs.c` & `lab7zad2funcs.h`**: Core logical functions handling raw binary writing (`fwrite`) and reading (`fread`) of structural objects to detect specific quadrant points (e.g., points with both positive coordinates).
* **`lab7zad2menu.c` & `lab7zad2menu.h`**: Dedicated logic for the binary application dashboard.

---

## 🛠️ How to Compile and Run
To compile any single-file lab task using `gcc`:
```bash
gcc lab2zad2b.c -o program -lm
./program
