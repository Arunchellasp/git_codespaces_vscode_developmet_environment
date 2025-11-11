# GCC C Compiler Installation Guide

## Installation Steps

### 1. Update Package Lists
```bash
sudo apt update
```

### 2. Install Build Essential Package
```bash
sudo apt install build-essential
```

This package includes:
- GCC (GNU Compiler Collection)
- G++ (C++ compiler)
- Make and other development tools

## Verification

### Check GCC Installation
```bash
gcc --version
```

Expected output should show GCC version information.

### Test with a Simple C Program

#### Create a test file
```bash
echo '#include <stdio.h>
int main() {
    printf("Hello, World!\n");
    return 0;
}' > test.c
```

#### Compile the program
```bash
gcc test.c -o test
```

#### Run the compiled program
```bash
./test
```

Expected output: `Hello, World!`

#### Clean up test files
```bash
rm test.c test
```

## Basic GCC Usage

### Compile a C program
```bash
gcc filename.c -o outputname
```

### Compile with warnings enabled
```bash
gcc -Wall filename.c -o outputname
```

### Compile with debugging information
```bash
gcc -g filename.c -o outputname
```

## Troubleshooting

If installation fails, ensure you have:
- Active internet connection
- Sufficient disk space
- Proper sudo privileges

For additional help, run:
```bash
man gcc
```