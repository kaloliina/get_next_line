# get_next_line

## Project Overview

Get Next Line is a project that involves creating a function to read a line from a file descriptor. The goal of this project was to understand and implement the functionality of reading lines from a file descriptor, handling various edge cases such as empty lines, lines ending with a newline character, and lines that are too long to fit into the buffer.

## My Approach

I began by reading about input-output system calls and how to open a file for reading into a file descriptor. I began building the function step by step, first making sure I could read one line properly, then the entire file. After I was satisfied with that, I proceeded to implement how to handle the different buffer sizes while still reading the entire line. This project felt rather complicated to me as it was difficult to divide the tasks into bite-sized pieces, which then led to me going back and forth in code to ensure the edge cases and possible errors were covered.

## Learnings

- File Handling: Get Next Line taught me a lot about working with file descriptors and reading from files efficiently.

- Error Checking: This project really drove home the importance of robust error checking, especially when dealing with memory allocation. I learned to always ensure proper cleanup in case of failures to prevent memory leaks and keep my program stable.

## Future Directions

I would love to review this implementation once more. I realized in later projects that my get_next_line function returns NULL both when the file is fully read and if there's a memory allocation issue. This makes it problematic because I don't have a clean way to check whether the file was read successfully until the end or if it encountered an error.

## How to Run the Project

- Setup Instructions: To use my Get Next Line implementation, clone the repository and compile the source files using the provided Makefile.

- Usage Examples: Include my Get Next Line function in your projects by linking against the compiled library and using it in your code.
