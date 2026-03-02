Beginner-Friendly Linux

## SHELL?

- Before starting to learn about the Linux command line, we have to know some terminology and facts.

- The shell is the command line interpreter, meaning that it takes the commands that you enter and sends them to the operating system to perform (execute).

- And so to make things clear, The shell is what actually handles the commands.

- The **shell is the default interface to Linux.**

## The Terminal

- On the other hand, The **Terminal** is just a graphical interface to the shell. In other words, We access the shell through our terminal in a **GUI (Graphical User Interface)** environment.

# Github codespaces setup

- We are using github VScode codespaces to practice Linux Commands.

1) Login to github > Create repo > create a file in it (i.e - readme.md). 

## why  we need to create a file?
Because to create codespace need atleast one file in the repo. Otherwise, it'll not allow to create codespace.

2) Click on Create Codespace (wait until VS Code opens).

3) To menu: Terminal > New terminal.
    Test: pwd

4) **Linux practice structure:**
Run in terminal:
                mkdir -p Linux-basics/day1
                cd Linux-basics/day1
Check:
        pwd
        ls

5) **Git workflow** (Most IMP)

---[run in terminal in day1 directory]----

Git status check: --> git status 

It shows: Untracked files.

6) Run in terminal: --> git add .

check: --> git status

Now should show: Changes to be committed.

7) **Only on FIRST TIME (Identity Set)**

Note: If haven't done this before. Then only follow this step.

Run: 
    git config --global user.name "Your_Name"

    git config --global user.email "Your_Email_Id"

(Do this only one time)

8) Commit

Run:
    git commit -m "Linux practice day1"

9) **Push** (IMP)

Run:
    git push -u origin main

Note: On first push only we use : -u origin main

----Successfully github codespace setup done-------------------

## Daily habit (This build GREEN Graph)

Run:
    git add .
    git commit -m "Give any name or write what you have done"
    git push

    



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

