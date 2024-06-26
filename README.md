# Manufacture

Manufacture is a command-line tool designed to help developers manage and create files with specified names and types efficiently. It streamlines file handling tasks, making it easier to organize project files.

## Features

- Create files with specific names and types
- Rename files with optional backup
- Change file permissions and ownership
- Create directories
- Display file information
- Compress directories
- Easy installation via pip
- Simplified file management from the terminal

## Installation

You can install Manufacture using pip:

```bash
pip install manufacture
```

## Usage

```bash
# Create a new file with a specified name
manufacture create <filename>

# Rename a file with an optional backup
manufacture change <oldname> <newname> [--backup]

# Change file permissions
manufacture permissions <filename> <permissions>

# Change file ownership
manufacture ownership <filename> <owner> <group>

# Create a new directory
manufacture directory <dirname>

# Display information about a file
manufacture info <filename>

# Compress a directory
manufacture compress <directory> --output=<output>
```

## Examples

Create a Python file:
```bash
manufacture create my_script.py
```
Rename a file with backup:
``` bash
manufacture change oldname.txt newname.txt --backup
```

Change file permissions to read, write, and execute for the owner:
```bash
manufacture permissions my_script.py 755
```
Change file ownership to user john and group developers:
```bash
manufacture ownership my_script.py john developers
```

Create a new directory:
```bash
manufacture directory my_project
```

Display information about a file:
```bash
manufacture info my_script.py
```
Compress a directory:
```bash
manufacture compress my_project --output=my_project.zip
```

