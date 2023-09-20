**Simple Shell Team Project**

This project was completed using the C language and Shell Betty linter.

**General Requirements for the Project**

- All files are compiled on Ubuntu 20.04 LTS using gcc with the options -Wall -Werror -Wextra -pedantic -std=gnu89.
- All files end with a new line.
- A README.md file at the root of the folder of the project is mandatory.
- The Betty style is used to check the code using betty-style.pl and betty-doc.pl.
- The Shell should not have any memory leaks.
- There are no more than 5 functions per file.
- All header files are include guarded.

**Description**

The `hsh` is a simple UNIX command language interpreter that reads commands from either a file or standard input and executes them.

**How `hsh` Works**

1. Prints a prompt and waits for a command from the user.
2. Creates a child process in which the command is checked.
3. Checks for built-ins, aliases in the PATH, and local executable programs.
4. The child process is replaced by the command, which accepts arguments.
5. When the command is done, the program returns to the parent process and prints the prompt.
6. The program is ready to receive a new command.
7. To exit: press Ctrl-D or enter "exit" (with or without a status).
8. Works also in non-interactive mode.

**Compilation**

```bash
gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh
