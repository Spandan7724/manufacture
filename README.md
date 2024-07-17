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
- Short-form commands for quicker usage
- Ability to handle multiple filenames or directories in a single command

## Installation

You can install Manufacture using pip:

```bash
pip install manufacture
```

## Usage

```bash
# Create a new file with a specified name
manufacture create <filename>
manufacture -c <filename>

# Create a new directory
manufacture directory <dirname>
manufacture -d <dirname>

# Rename a file with an optional backup
manufacture change <oldname> <newname> [--backup]
manufacture -ch <oldname> <newname> [--backup]

# Change file permissions
manufacture permissions <filename> <permissions>
manufacture -p <filename> <permissions>

# Change file ownership
manufacture ownership <filename> <owner> <group>
manufacture -o <filename> <owner> <group>

# Display information about a file
manufacture info <filename>
manufacture -i <filename>

# Compress a directory
manufacture compress <directory> --output=<output>
manufacture -z <directory> --output=<output>
```

## Examples

Create one or multiple files:
```bash
manufacture create script1.py script2.rs
manufacture -c main.go test.rs
```

Create a new directory:
```bash
manufacture directory dir1 dir2
manufacture -d dir1 dir2
```

Rename a file with backup:
``` bash
manufacture change oldname.txt newname.txt --backup
manufacture -ch oldname.txt newname.txt --backup
```

Change file permissions to read, write, and execute for the owner:
```bash
manufacture permissions my_script.py 755
manufacture -p my_script.py 755
```

Change file ownership to user jack and group developers:
```bash
manufacture ownership my_script.py jack developers
manufacture -o my_script.py jack developers
```

Display information about a file:
```bash
manufacture info my_script.py
manufacture -i my_script.py
```

Compress a directory:
```bash
manufacture compress my_project --output=my_project.zip
manufacture -z my_project --output=my_project.zip
```

