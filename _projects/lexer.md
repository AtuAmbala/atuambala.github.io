---
layout: single
title: "Lexer Analyzer"
subtitle: "Building a lexer Analyzer"
date: 2024-07-18
permalink: /projects/lexer/
author_profile: true
read_time: true
---


This project is a **lexer analyzer** built with **Flex and C**, which represents the foundational stage of building a compiler. The purpose of this tool is to read source code from a file and translate it into a stream of **tokens**. This process, known as lexical analysis, is a crucial first step before the code can be parsed and compiled.

My work on this project involved:

* **Tokenization:** I defined a comprehensive set of rules in `lexer.l` to recognize different language constructs, including data types, commands, conditional statements, identifiers, and various operators.
* **Finite Automata Implementation:** This project demonstrates the practical application of theoretical computer science concepts like deterministic finite automata (DFA), which defines the rules for token recognition.
* **Automated Build Process:** A `Makefile` automates the entire build process, compiling the Flex rules into C code and creating an executable that can be run on the provided input file.

By building this lexer, I gained a deeper understanding of how programming languages are structured and how a compiler breaks down source code into its most basic components. This project showcases my ability to implement fundamental concepts from computer science and systems programming.

See a video demonstration of the project [here](https://www.loom.com/share/9213217a6b7b4fcd99e6f5ba08176515?sid=4bf1aadc-353e-4fd9-8260-596ff2984332) and explore the full codebase on [GitHub](https://github.com/AtuAmbala/Projects/tree/main/lexerAnalyzer/).
