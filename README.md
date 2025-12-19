# Mini Unix Shell in C

A simple Unix-like shell implemented in C to understand how operating systems
create and manage processes.

## Features
- Interactive command-line interface (REPL)
- Execute external commands using fork + exec
- Built-in commands:
  - cd
  - help
  - exit
- Dynamic memory allocation for input handling
- Graceful error handling

## How It Works
1. Reads user input from stdin
2. Tokenizes input into command and arguments
3. Creates a child process using fork()
4. Executes the command using execvp()
5. Parent waits for child process using wait()

## Example
```bash
shell> ls -l
shell> cd ..
shell> pwd

