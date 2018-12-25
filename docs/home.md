# Intro to System Programming

As a pilot offering, the title of this course is admittedly vague. System software is an overloaded term that can include: operating systems, distributed systems, parallel systems, programming language compilers/runtimes/interpreters, device drivers, utility software, and more.

In this course, you will:

1. Gain experience with compiled systems languages.
    - Learn enough C to appreciate its primary strengths and dangers.
        - Pointers and the perils of non-type safe languages
        - Heap memory management (`malloc`, `calloc`, `free`)
        - System calls (Standard and File I/O)
    - Learn Rust, a modern system programming language, with an emphasis on the ideas it inherits from notable earlier languages.
        - ML-inspired type inference and pattern matching
        - C++ inspired "zero-cost abstractions"
        - Rust's own type safe value ownership model and borrow checker
    - Deepen your understanding of the application programming languages you know.
        - Understand garbage collection algorithms and implications in memory managed runtimes
        - Use `Optional` to eliminate `null` pointer exceptions at compile time
        - Reason critically about mutability and referential transparency
        
2. Implement theoretical machines as an introduction to programming language systems software.
    - `grep` - Finite State Machines and Regular Languages
    - `dc` and `bc` - Stack Machine calculators from the original unix
    - `scheme` - A programming language rooted in Lisp and lambda calculus that can simulate any Turing Machine 

3. Practice software engineering in a traditional, Unix-like operating system environment.
