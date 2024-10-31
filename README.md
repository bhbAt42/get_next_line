```

Get Next Line
This project is part of the 42 school curriculum, aimed at enhancing your understanding of file handling and reading in C. get_next_line is a function that reads a line from a file descriptor and returns it. Successive calls to this function should allow you to read the entire content of a file, one line at a time.

Table of Contents
Installation

Usage

Function Prototype

Project Rules

License

Installation
To clone and compile the project, follow these steps:

sh
git clone https://github.com/yourusername/get_next_line.git
cd get_next_line
make
Usage
To use the get_next_line function in your own projects, include the following header file in your C source files:

c
#include "get_next_line.h"
Then, compile your project with the get_next_line.a file generated during the installation:

sh
gcc -L. -lgnl yourfile.c -o yourprogram
Function Prototype
c
char \*get_next_line(int fd);
Parameters:

fd: The file descriptor to read from.

Return value:

The content of the read line, or NULL if there's nothing more to read or an error occurs.

Project Rules
Your project must be written in C.

Your project must adhere to the Norm. If you have bonus files/functions, they are included in the norm check.

Your functions should not quit unexpectedly (segmentation fault, bus error, double free, etc.), except in the case of undefined behavior.

All heap-allocated memory space must be properly freed when necessary. No leaks will be tolerated.

You must submit a Makefile that will compile your source files. The Makefile should include the flags -Wall, -Wextra, and -Werror and must not relink.

Your Makefile must contain the rules $(NAME), all, clean, fclean, and re.

To submit bonuses, you must include a bonus rule in your Makefile that adds the various headers, libraries, or functions that are forbidden in the main part of the project. Bonuses must be in a different file \_bonus.{c/h}.

If the project allows using your libft, you must copy its sources and Makefile into a libft folder. Your project’s Makefile must compile the library using its Makefile, then compile the project.

You are encouraged to create test programs for your project. They won't be submitted or graded but will help you test your work and your peers’ work.

Submit your work to the assigned git repository. Only work in the git repository will be graded.
```
