Beginner-Friendly Linux

## SHELL?

- Before starting to learn about the Linux command line, we have to know some terminology and facts.

- The shell is the command line interpreter, meaning that it takes the commands that you enter and sends them to the operating system to perform (execute).

- And so to make things clear, The shell is what actually handles the commands.

- The **shell is the default interface to Linux.**

## The Terminal

- On the other hand, The **Terminal** is just a graphical interface to the shell. In other words, We access the shell through our terminal in a **GUI (Graphical User Interface)** environment.

## Github codespaces setup

- We are using github VScode codespaces to practice Linux Commands.

- 

## What is touch?

The touch command is used to create empty files in Linux.

It can also update the timestamp of existing files.

## Syntax
touch filename

## What it will do

- Creates empty file
- Can create multiple files

---
## Examples

### Create single file
touch fileA.txt

### Create Multiple files
touch file.txt file1.txt file2.txt

---
## What is mv?

mv is used to rename and move the files and folders.

## Syntax
mv sourcefile destinationfile

- Sourcefile: which file you want to rename/move.

- Destinationfile: where you have to move inside or what you to rename it for.

## Examples

### Rename files
mv file1.txt file.txt

Explaination: File1 will overwrtite the file. Here only **file1** name is changes to **file**. 
Contents of file1 unchanged but file contents erased.

Remember: Whenever using mv between two files check whether do you want contents of destination file or not.

