 **DSL Compiler Simulation – Conditional Expression**
 
 Project Overview

This project implements a **mini compiler simulation** for a simple **Domain-Specific Language (DSL)** using the C programming language. It demonstrates how a compiler processes a **conditional (ternary) expression** step-by-step.

 Objective

* To simulate compiler phases using a simple DSL
* To evaluate a conditional expression:
  **`max = (a > b) ? a : b`**
* To demonstrate lexical analysis, parsing, semantic analysis, and code generation

 Compiler Phases Implemented

🔹 1. Lexical Analysis

* Identifies tokens:

  * Identifiers → `a`, `b`, `max`
  * Numbers → `8`, `5`
  * Operator → `>`
  * Conditional symbols → `?`, `:`

🔹 2. Syntax Parsing

* Recognizes valid expression:

```text
max = (a > b) ? a : b
```
🔹 3. Semantic Analysis

* Checks:

  * Variables are valid
  * Data types are integers
  * Conditional expression is logically correct

 🔹 4. Intermediate Code Generation

```text
if a > b goto L1
t1 = b
goto L2
L1: t1 = a
L2: max = t1
```

 Sample Input

```text
a = 8
b = 5
max = a > b ? a : b
```

 Sample Output

```text
Final Output:
max = 8
```

 Technologies Used

* **C Programming Language**
* Standard library: `stdio.h`

 Project Structure

```text
DSL-Compiler-Conditional/
├── src/        → C source code
├── output/     → Execution screenshots
├── docs/       → Explanation document
├── test/       → Input file
└── README.md
```

 How to Run

1. Open the `.c` file in any C compiler (Dev-C++, Code::Blocks, or online compiler)
2. Compile the program
3. Run the executable
4. View output in the console

 Key Features

* Simulates real compiler phases
* Demonstrates conditional (ternary) logic
* Simple and easy-to-understand implementation
* Structured and readable output

 Conclusion

This project provides a clear understanding of how compilers process conditional expressions. It demonstrates the transformation of input code through different phases into a final result.

 Author

**Name:** Tippluri Jahnavi, **Reg NO:** RA2311026050242, **Course** BTech CSE AIML- D
