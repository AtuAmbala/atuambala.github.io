---
layout: single
title: "lopeShell"
subtitle: "A custom shell with a hierarchical file management system, similar to Unix/Linux"
date: 2024-06-27
permalink: /projects/lopeShell/
author_profile: true
read_time: true
---

This project is a custom shell named LopeShell, built in **C** to provide a hands-on understanding of fundamental operating system concepts. It replicates core functionalities of a Unix/Linux shell, focusing on **file and process management**. My goal was to create a robust and functional shell that can execute user commands, manage processes, and handle file operations efficiently.

Key features of this project include:

* **Dual-mode Operation:** LopeShell supports both **interactive mode** for real-time user input and **batch mode** for executing a series of commands from a script file.
* **Comprehensive File System Management:** The shell handles a variety of file and directory operations, including creating, renaming, moving, and deleting files and directories. It also supports **recursive operations**, such as duplicating an entire directory tree.
* **Process Management and Scheduling:** A key component is the implementation of a **round-robin scheduler** with priority handling. This demonstrates an understanding of how to manage multiple processes and ensure fairness by preventing resource starvation.
* **Advanced Features:** The shell provides a `history` command to track past commands and an `info` command to retrieve detailed metadata about files and directories.

This project showcases my ability to work with **low-level systems programming**, demonstrating a strong grasp of memory management and an in-depth understanding of how operating systems handle file systems and processes. It was a great exercise in building a core piece of software from the ground up, providing valuable insights into the architecture of modern operating systems.

<img width="1190" height="200" alt="image" src="https://github.com/user-attachments/assets/7354d37b-7d8c-4a21-83dd-c41e88809d15" />


See a demo of the shell in action [here](https://www.loom.com/share/c320cd3f5d154cde9abfa8838f42c3f7?sid=598647ea-a6f5-41f2-aa85-b86b4f23ee2f) and explore the full codebase on [GitHub](https://github.com/AtuAmbala/CST-315/tree/main/Project6%3AFileSystemManager.git).

***

### LopeShell Technical Overview

To give you a better sense of the complexity and scope of the project, here are the key objectives I focused on:

* **Command Parsing:** The shell processes user input, identifying commands and arguments to correctly execute the requested operations.
* **Built-in Commands:** I implemented 13 different commands, from basic file creation to advanced search and directory listing.
* **Memory and Process Handling:** The project required careful management of memory and process states to ensure efficient resource utilization and prevent leaks or other runtime issues.
* **Error Handling:** The shell provides clear feedback to the user when a command fails, such as when a file or directory already exists.
