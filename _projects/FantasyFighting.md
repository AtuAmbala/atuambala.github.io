---
layout: single
title: "Fantasy Fighting Game"
subtitle: "A one player game where a you build out your loadout and battle a beast"
date: 2023-04-23
permalink: /projects/fantasyfighting/
author_profile: true
read_time: true
---

This is a **C++ console-based game** I built to demonstrate a deep understanding of object-oriented programming (OOP). The game pits a human player against a computer-controlled beast in a turn-based battle, but it's more than just a simple game—it's a showcase of foundational software design principles in practice.

The project's architecture is a prime example of **composition and inheritance**. As shown in the UML diagram, the game's core logic is structured around a network of interconnected classes:

* **Player Hierarchy:** The `Human` and `Beast` classes inherit from a base `Player` class, ensuring consistent behavior while allowing for unique attributes and abilities for each character.
* **Item System:** The game's economy is powered by a `Store` class that is composed of various items. These items—`Weapons`, `Armors`, and `Potions`—each have their own base class and specialized subclasses (e.g., `Sword`, `Club`, `Gun`), demonstrating how to manage item-specific logic while maintaining a unified structure.
* **Core Logic:** Classes like `Arena` and `Data Access` handle the main game loop, battle mechanics, and the crucial ability to **save and load game states**. This feature highlights the ability to manage file I/O and serialize complex game data.

By implementing this structure, I focused on creating a **robust, scalable, and memory-safe** application. The result is not just a playable game, but a clear demonstration of how to build a clean and extensible C++ codebase.

---
<img width="959" height="660" alt="Fantasy_Game_UML" src="https://github.com/user-attachments/assets/2787aafd-a20e-4ec5-9283-4c7e211e494b" />


**Want to see it in action?** Check out the full [demo video](https://www.youtube.com/watch?v=Bh_nOo4jjD4), or dive into the code on the project's [GitHub repository](https://github.com/AtuAmbala/Projects/tree/main/FantasyFightGame).
