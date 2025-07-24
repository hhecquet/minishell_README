# minishell

> [!IMPORTANT]
> None of my code is publicly available here, but if you're a recruiter, I'd be happy to share it with you upon request.

<p align="center"> 
<img width="317" height="270" alt="Screenshot from 2025-07-23 15-19-50" src="https://github.com/user-attachments/assets/1803b076-8d23-4e6a-8c6e-c7284d36a31a" />
</p>

The ***minishell*** project is a fundamental exercise at 42 where I built a simplified Unix shell from scratch. The goal was to create a command-line interpreter capable of parsing and executing commands, managing processes, and handling environment variables, mimicking the behavior of common shells like bash or zsh.
This project deepened my understanding of how shells work under the hood and the intricacies of process management and command parsing in C.

What I had to do:
* Implement a command-line prompt that continuously reads user input
* Parse the input to separate commands, arguments, and handle quotes and escape characters
* Execute built-in commands like `cd`, `echo`, `pwd`, `env`, `export`, `unset`, and `exit`
* Launch external programs by creating child processes using fork and execve
* Manage environment variables, including passing them correctly to child processes
* Handle redirections (`>`, `<`, `>>`) and simple pipes (`|`) between commands
* Properly manage signals such as SIGINT and SIGQUIT to control the shell behavior during input and child execution
* Implement memory management to avoid leaks during parsing and execution

To achieve this, I had to:
* Parse and tokenize complex command lines accurately, respecting quotes and spaces
* Use system calls like fork, execve, waitpid, and pipe effectively
* Build a modular codebase separating parsing, execution, and built-in command handling
* Handle errors gracefully and provide meaningful feedback to the user

What I Learned:
* The inner workings of Unix shells and how commands are processed and executed
* Process creation and management with fork, execve, and waitpid
* Implementing robust command parsing that respects shell syntax
* Handling I/O redirections and piping between processes
* Signal handling to manage user interruptions and control flow
* Writing maintainable, modular C code that mimics real-world software

Minishell was a deep dive into system programming and process control. It strengthened my understanding of how shells interpret commands, interact with the OS, and manage processes, laying a solid foundation for advanced system-level programming.

Project done with [heperez](https://github.com/hdprz)
