# ft_printf

`ft_printf` is a custom implementation of the standard C library function `printf`. This project demonstrates the ability to understand and recreate the functionality of `printf` while adhering to specific constraints, such as avoiding the use of standard library functions.

## Features

- Supports a subset of standard `printf` functionality.
- Handles various format specifiers, such as `%c`, `%s`, `%d`, `%i`, `%u`, `%x`, `%X`, and `%%`.
- Custom implementation of string manipulation and number conversion functions.
- Adheres to memory management best practices.

## Language and Tools

This project is written in **C** and uses a **Makefile** for compilation.

### Language Composition

- **C**: 86.5%
- **Makefile**: 13.5%

## Getting Started

### Prerequisites

To compile and run the project, you need:

- A C compiler (e.g., `gcc`, `clang`).
- `make` utility installed on your system.

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/amrire/ft_printf.git
   cd ft_printf
   ```

2. Compile the project using the Makefile:

   ```bash
   make
   ```

### Usage

After building the project, you can test the `ft_printf` function by writing a simple C program that includes the `ft_printf.h` header and links against the compiled library.

Example:

```c
#include "ft_printf.h"

int main(void) {
    ft_printf("Hello, %s! The number is %d.\n", "world", 42);
    return 0;
}
```

Compile and run:

```bash
gcc -o test_program test_program.c libftprintf.a
./test_program
```

### Cleaning Up

To clean the compiled files, run:

```bash
make clean
```

To clean all compiled files and the library, run:

```bash
make fclean
```

## Testing

Tests for the `ft_printf` implementation are located in the repository. You can run them to verify the functionality:

```bash
make test
```

## Project Structure

- **src/**: Contains the source code files.
- **include/**: Contains the header files.
- **Makefile**: Automates the build process.
- **tests/**: Contains test cases for the project.
