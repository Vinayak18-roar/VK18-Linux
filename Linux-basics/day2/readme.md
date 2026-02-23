Beginner-Friendly Linux
# Day 2 - touch and mv Commands

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

## Practiced:

- Creating file using: touch
- rename files using: mv

## command mkdir
mkdir: It's used to create folders.

## synatx

mkdir <foldername>

## Examples

**Single folder creation**.

mkdir <foldername>

Ex: mkdir dir1

**Multiple folder creation**

mkdir <folder1> <folder2> <folder3>

ex: mkdir dir1 dir2 testdir

## mv on folders

- To rename or move folders.

## Syntax

mv sourcefile destinationfile

## examples

mv dir1 testdir

explaination: We placed **dir1** folder into **testdir** folder.