# Little Languages and Systems

System programming is an overloaded term that can include: operating systems, distributed systems, parallel systems, programming language compilers/runtimes/interpreters, device drivers, utility software, and more. Classically, these programs are written in "systems languages" like C (1972-) and C++ (1985-); Rust (2010-) is a modern entrant with a head full of steam.

COMP590 focuses on systems that 

In this course, you will:

1. Implement the essences of practical, historically significant systems utilities. Each has its own little language and is founded upon theoretical computing machines.
    - `dc` (1969) a calculator whose simple, reverse-polish notation language commands a virtual stack machine. 
    - `bc` (1975), the successor to `dc`, is an infix-based context free language needing a  pushdown automata equivalent to parse. It will be implemented, as it was historically, as a frontend translator for `dc`.
    - `grep` (1974) is a regular expression pattern matching tool still widely used today. Its implementation will construct and simulate a non-deterministic finite state machine.
    - `scheme` (1975) is a functional programming language rooted in Lisp and lambda calculus that can simulate any Turing Machine. It will be implemented as a basic read-evaluate-print-loop (REPL) interpreter.

2. Gain experience with compiled systems languages.
    - Learn enough C to appreciate its strengths and dangers.
        - Pointers and the perils of type-unsafe languages
        - Heap memory management (`malloc`, `calloc`, `free`)
        - System calls (Standard and File I/O)
    - Learn Rust, a modern system programming language, with an emphasis on the ideas it inherits from notable earlier languages.
        - ML-inspired type inference and pattern matching
        - C++ inspired "zero-cost abstractions"
        - Rust's own type safe value ownership model and borrow checker
    - Deepen your understanding of the application programming languages you know.
        - Understand garbage collection algorithms and implications in memory managed runtimes
        - When and how to avoid the use of `null` and  costly exception handling
        - Reason critically about mutability and referential transparency
        
3. Practice software engineering in a traditional, Unix-like operating system environment to gain fundamental skills and knowledge.
    - Gain proficiency with a version control system (`git`)
    - Employ the facilities of a shell (`bash`)
        - Clarity on `stdin`, `stdout`, `stderr`
        - Establish using piping and redirection