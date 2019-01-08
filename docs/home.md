-----

![Little Languages](/img/title.jpg)

-----

Computer scientists and software engineers depend on tools that interpret Little Languages ([Bentley, UNC '76](http://staff.um.edu.mt/afra1/seminar/little-languages.pdf)) frequently in their day-to-day work: command-line shells, project build system configurations, regular expressions, utility programs, documentation markup languages, modal text editors, and so on. As these languages are numerous and domain-specific, our focus will be on their first principles, common challenges, implementations, and limitations.

This course will explore the interpretation and applications of little languages through case studies on standard programming environment tools with historical significance, such as `grep`,  `make`, `bash`, `vim`, and more. This course highlights important ideas in computational theory through direct, pragmatic applications in text pattern matching and structured language processing.

You will gain experience working in a systems language appropriate for implementing command-line tools with their own little languages. You will gain comfort working in a Unix-like programming environment and knowledge of its standard tooling and utilities. You will learn to make use of a Unix-like operating system's facilities and APIs for file system input/output, process management, and memory management.

In this course, you will:

1. Implement the essences of practical, historically significant Unix utilities, each with its own little language.
    - `dc` (1969) a calculator whose simple, reverse-polish notation language commands a virtual stack machine. It is the oldest little language in Unix.
    - `bc` (1975), the successor to `dc`, is an infix-based context free language needing a  pushdown automata equivalent to parse. It will be implemented, as it was historically, as a frontend translator for `dc`.
    - `grep` (1974) is a regular expression pattern matching tool still widely used today. Its implementation will construct and simulate a non-deterministic finite state machine.
    - `sh` (1977) the interpretation of Bourne's shell, or command-line interpreter, introduces fundamental operating systems concepts.

2. Be introduced to, or reinforce your understanding of, first principles in computational theory and structured language processing.
    - Lexical analysis through tokenization and parsing
    - Regular languages
    - Finite state machines and non-deterministic finite state machines (automata) 
    - Context-free languages
    - Stack machines and pushdown automata
    - Parser generators
    - Language translation

3. Gain experience with compiled systems languages appropriate for implementing command-line utilities which interpret little languages.
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
        
4. Practice software engineering in a Unix-like operating system programming environment to gain fundamental skills and knowledge.
    - Employ the facilities of a shell (`bash`)
        - Clarity on `stdin`, `stdout`, `stderr`
        - Use piping and redirection to compose programs together
    - Make use of a historical build system and its configuration file (`make`)
    - Gain comfort operating a standard text editor and its command language (`vim`)
    - Gain exposure to powerful text processing utilities and their little languages (`sed`, `awk`, `grep`)
    - Gain proficiency with a version control system (`git`)
