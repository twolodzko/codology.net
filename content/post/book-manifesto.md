---
title: "Book Manifesto"
date: 2018-09-26T21:03:14+02:00
draft: true
---

Nobody should start to undertake a large project. You start with a small trivial project, and you should never expect it to get large. If you do, you’ll just overdesign and generally think it is more important than it likely is at that stage. Or worse, you might be scared away by the sheer size of the work you envision. So start small, and think about the details. Don’t think about some big picture and fancy design. If it doesn’t solve some fairly immediate need, it’s almost certainly over-designed. And don’t expect people to jump in and help you. That’s not how these things work. You need to get something half-way useful first, and then others will say “hey, that almost works for me”, and they’ll get involved in the project.

        — Linus Torvalds

- Very high quality code of he final results
- Clean code architecture
- Almost production ready
- With documentation
- Show also unclean code on the step to clean code
- No dumbing down
- Minimual theory
- Real runnable code
- From scratch, as little dependencies as possible
- No skipping of anything!
- written with tests first and without 3rd-party libraries.
- not about theory, its focus is runnable, working code.
- Clarity of explanation
- Show how it is build step by step, not just the result
- Break through layers of abstraction
- Identify incorrect assumptions
- complex programs are constructed by building, step by step, computational objects of increasing complexity
- incremental development and testing
- a modern, non-naive implementation
- reasonably fast
- foundational
- step by step, show challenges and tradeoff and decisions
- Accuracy in words
- Simple is not easy (https://www.infoq.com/presentations/Simple-Made-Easy)
- great introduction to the subject
- no CS degree, highly interested in interpreters and compilers, but intimidated by the existing literature.
- Showing the path and the why, not just the matured end resutl (ex of database)
- "How do you know this is correct?"
- Intuitive Understanding
- design decisions history
- untangle things : problem decomposition (how to teach that? is there no book or course focused only on that?)
- Code simplicity (http://www.sromero.org/wiki/_media/programacion/tutoriales/code_simplicity_summary.pdf)
- Clean code
- Software design
- designing boundaries
- Make a bee line to your target and expand however you want (https://www.youtube.com/watch?time_continue=4&v=jviNpRGuCIU)
- vizualisation of execution
- formal spec https://www.hillelwayne.com/post/tla-messages/
- how you might design one such version control system (VCS) and the reasoning behind those design choices
- Zéro dependancy
- This is not theory: it shows how a given compiler is build, it doesn't explain all the ways you can build a compiler. It explain some of the choices, but no all the variations.

Building an xxx in yyy
Coding
Programming
Writing
developing

from scratch
from the ground up
from the Bottom Up

Topics:

- OS
  - multitask
  - https://github.com/dspinellis/unix-history-repo
- File System
- Language
  - Strongly or weakly typed?
  - Garbage Collected?
  - Functional, OO, "normal", logic
- Compiler
  - http://web.stanford.edu/class/cs143/
  - https://news.ycombinator.com/item?id=8558822
  - Target ARM plateform?
- Write a version of the compiler in the language and have it compile itself
- parser
  - https://news.ycombinator.com/item?id=18391128
- interpreter
  - http://www.craftinginterpreters.com/
  - https://news.ycombinator.com/item?id=12553591
    - https://gpfault.net/posts/most-important-project.txt.html
- Type system
  - https://news.ycombinator.com/item?id=15034089
  - http://cs.brown.edu/courses/cs173/2012/book/types.html
- Memory allocators
- Linkers and loader
  - https://news.ycombinator.com/item?id=18424233 (Linkers and Loaders (1999))
- JIT
- REPL
- Database
- SQL
  - https://news.ycombinator.com/item?id=15034285
  - https://news.ycombinator.com/item?id=18363760
  - https://www.cockroachlabs.com/blog/building-cost-based-sql-optimizer/
- NoSQL
- Columnar
- Analytic oriented database
- Text Editor
- Shell
- Hardware: CPU/Computer
  - ARM?
  - PIC?
  - RISC V?
  - MMU
  - https://news.ycombinator.com/item?id=18413757 (How Many Computers Are in Your Computer?)
- Network
- Game: roguelike (https://www.youtube.com/watch?time_continue=4&v=jviNpRGuCIU)
- Log based database
- Profiler
- Debugger
- Streaming
- Event based
- Business Oriented (CRM, with invoicing, like gumroad)
- regex engine
  - https://news.ycombinator.com/item?id=12553591
- Benchmarking
  - https://blog.janestreet.com/core_bench-micro-benchmarking-for-ocaml/

Inspiration:

- https://news.ycombinator.com/item?id=18274235
- http://www.pbr-book.org/
- https://news.ycombinator.com/item?id=18277450
- https://blog.invisiblethings.org/2015/12/23/state_harmful.html (markdown to pdf)
- https://news.ycombinator.com/item?id=18282324
- http://aosabook.org/en/pypy.html
- https://news.ycombinator.com/item?id=18315292
- http://gameprogrammingpatterns.com/

https://www.ybrikman.com/writing/2014/05/29/must-see-tech-talks-for-every-programmer/

improve writing clarity: use debating society?

Books

https://pragprog.com/book/tpdsl/language-implementation-patterns

https://news.ycombinator.com/item?id=13079611

The way I would sum up interpreters and compilers, trying to put it as concisely as possible:
Step 1. Write a program that reads the input program into a data structure that exactly represents the language. You just wrote a parser.

Step 2. Write a program that operates on the data structure from (1) to execute the program. You just wrote an interpreter.

Step 3 (Optional): Write a program that converts the data structure from (1) into a different data structure that you can interpret more efficiently. You just wrote an optimizer.

Step 4 (Optional): Keep iterating on (3) until the output of your optimizer is machine code. You just wrote a compiler.

Not saying the above obviates the need for a book like this one (at all), I just had never thought of it in quite this way and wanted to write it down. :)

The author seems to be doing a good thing. Like he said, most of the write-ups on this subject are either ultra-heavy with theory or basically nothing with code examples. Doing interpreters piece-by-piece like in SICP or The Little Schemer series in an accessible language gradually giving them the code and theory they need is a good idea.
