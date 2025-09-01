---
layout: single
title: "Compiler"
subtitle: "Building a custom compiler from the ground up"
date: 2024-12-15
permalink: /projects/compiler/
author_profile: true
read_time: true
---

This project is a fully functional **compiler** for a custom language (referred to as C-- or `cmm`), built from scratch in **C** using **Flex** and **Bison**. The compiler processes source code through a series of stages—lexical analysis, syntax analysis, semantic analysis, and code generation—to produce executable **MIPS assembly code**. This project represents a comprehensive application of core computer science principles, from theoretical concepts to practical implementation.

---

### Core Compiler Functionality

The compiler is a complete toolchain that transforms high-level code into low-level machine instructions. My work involved developing each of the following components:

#### 1. Lexical Analysis (`lexer.l`)
This initial phase uses **Flex** to tokenize the C-- source code, identifying keywords, identifiers, and various operators. This process is a practical application of **Deterministic Finite Automata (DFA)**, which defines the rules for token recognition.

#### 2. Syntax and Semantic Analysis (`parser.y`, `AST.c`, `symbolTable.c`)
Using **Bison**, the compiler parses the token stream to check for proper syntax and builds an **Abstract Syntax Tree (AST)**. This is a crucial step for representing the program's structure. During this stage, **semantic analysis** is performed to check for type correctness, and a **symbol table** is built and managed to handle variable and function scope.

#### 3. Intermediate and MIPS Code Generation (`semantic.c`, `codeGenerator.c`)
The compiler generates a **Three-Address Code (TAC)** as an intermediate representation. This TAC is then used to produce final, optimized **MIPS assembly code**. I focused on translating high-level constructs, such as loops, conditional statements, and arithmetic operations, into efficient MIPS instructions.

---

### Key Features and Implementation Details

The compiler supports a wide range of features, showcasing advanced systems programming and algorithmic design skills:

* **Control Flow:** Implemented support for **`if-then` and `if-then-else` statements** and **`while` loops** to handle conditional and iterative logic.
* **Complex Data Types and Operations:** The compiler correctly handles **arrays**, including their declaration, assignment, and access. It also processes complex **arithmetic and logical Boolean expressions**, respecting the correct **order of operations**.
* **Functions and Scoping:** The compiler manages function declarations and calls, correctly handling **variable scope** to ensure that variables are accessed and modified in the intended context.
* **Performance Metrics:** The final compiler is efficient, with a recorded execution time of just 2.85 milliseconds. The generated MIPS code for a 168-line C-- program results in 840 lines of M
