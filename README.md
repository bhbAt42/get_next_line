# get_next_line

## 🎯 Project Overview

`get_next_line` is a function developed as part of the 42 school curriculum, designed to read a line ending with a newline character from a file descriptor. This project is crucial for understanding file handling, dynamic memory allocation, and string manipulation in C.

## 📌 Features

- Reads a single line from a file descriptor
- Handles multiple file descriptors simultaneously
- Manages different buffer sizes
- Works with standard input, files, and other file descriptors
- Memory efficient with dynamic allocation

## 🛠 Function Prototype

```c
char *get_next_line(int fd);
```

### Parameters
- `fd`: File descriptor to read from

### Return Values
- Returns a line read from the file descriptor
- Returns `NULL` when there is nothing left to read or an error occurs

## 🧠 Key Concepts

- Static variables
- Dynamic memory allocation
- File descriptor reading
- Buffer management
- Memory leaks prevention

## 🚀 Compilation

To compile the project, use the following flags:

```bash
gcc -Wall -Wextra -Werror -D BUFFER_SIZE=42 get_next_line.c get_next_line_utils.c
```

## 📦 Bonus Features

If implemented, bonus features might include:
- Handling multiple file descriptors
- Efficient memory management
- Minimal memory allocation

## 🔍 Usage Example

```c
int fd = open("example.txt", O_RDONLY);
char *line;

while ((line = get_next_line(fd)) != NULL) {
    printf("%s", line);
    free(line);
}
close(fd);
```

## ⚠️ Potential Challenges

- Handling different buffer sizes
- Managing static variables
- Preventing memory leaks
- Efficiently splitting lines

## 🏆 Learning Objectives

- Understand file reading mechanisms
- Practice dynamic memory management
- Improve string manipulation skills
- Learn about file descriptors and system calls

## 📝 Notes

- Ensure proper memory management
- Test with various buffer sizes
- Handle edge cases (empty files, large lines)

## 📊 Project Status

- Completed ✅
- Norminette compliant 📋
- Passes all mandatory tests 🧪

## 🤝 Contributing

Feel free to open issues or submit pull requests for improvements or bug fixes.

## 📄 License

This project is open-source. Please check the license file for details.
