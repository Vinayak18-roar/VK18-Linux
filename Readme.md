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

6) Run in terminal: 
                    
        --> git add .

    check: 
    
        --> git status

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

--------Successfully github codespace setup done-------------------

## Daily habit (This build GREEN Graph)

Run:

    git add .

    git commit -m "Give any name or write what you have done"

    git push


## LOCAL vs REMOTE

    Logic:

        Local: Laptop folder

        Remote: Google drive / Github

    Main topic:

        Local repository:

            It's your machine / codespaces. Where you do all edit, add, commit. This is known as local repository.

            Example:

                /workspaces/VK18-Linux

            - fast

            - Private to you

            - It will work on offline
        
        Remote repository:

            Which is stored in github.(like cloud copy) known as remote repository.

        Example:

            origin --> github.com/Vinayak18-roar/VK18-Linux

        - Cloud copy

        - backup
            

## Github ERROR Analyses:

- Whenever "git push" failed then, follow 3 steps:

1) Status check:

    Run:

        git status

2) Ahead/behind check:

    Check below messages after status check

    i. behind --> pull needed

    ii. ahead --> push needed

    iii. divereged --> rebase needed.

3) Three cases:

    Case 1: BEHIND (pull needed)

        Error message:

            Your branch is behind **origin/main** by 2 commits

        Meaning:

            - In remote, there is new commits.

            - In local there is no commits.

        Visual:

            Remote :

                A - B - C

            Local :

                A - B

        Solution:

            git pull --rebase

        Memory hook:
        
            Bheind = pull first

    Case 2: AHEAD (push needed)

        Error message:

            Your branch is ahead of **origin/main** by 1 commits

        Meaning:

            - Commited in local

            - Not pushed in remote.

        Visual:

            Remote:

                A - B

            Local:

                A - B - C

        Solution:

            git push
    
        Memory hook:

            Ahead = Push
    
    Case3: Diverged (rebase needed) --> VVIMP

        Error message:

            Your branch and **origin/main** have diverged

            or

            non-fast-forward

            or

            need to reconcile divergent branches

            or 

            failed to push some refs

        Meaning:(both - remote and local)

            - New commits in remote

            - local also has new commits.

            - Push rejected.

        Visual:

            Remote:

                A - B - R

            Local:

                A - B - L

                Here commit happened in both remote and local. Therefore, conflict chance is high.

            Solution:

                git pull --rebase

                git push

            Memory hook:

                Diverged = Reabse & push

4) Extra cases:

    1. Clean

    2. Not staged

    3. Staged

    4. Detached HEAD

    Case1: CLEAN

        Error message:

            Nothing to commit, working tree clean

        Meaning:

            - All commit is done.

            - May be push is pending

            - All already synced successfully

        Solution:

            Check Ahead/behind and based on this take a step.

    Csae2: NOT STAGED

        Error message:

            Changes not staged for commit :

            modified: Readme.md

        Meaning:

            - File changed

            - Not added to git

            - Git will not commit it

        Visual:

            working directory --> changed

            staging area --> empty

        Solution:

            git add .

            git commit -m "Write here what you have done"

            git push

        Memory hook:

            Modify --> Add first

    Case3: STAGED (ready to commit)

        Error message:

            Changes to be committed:

            newfile: file.txt

        Meaning: 

            - git add is done but haven't committed yet

        Visual:

            working --> staged

            commit --> pending

        Solution:

            git commit -m "message"

            git push

        Memory hook:

            Staged --> commit

    Case 4: Detached HEAD

        Error message:

            You are not currently on a branch
        
        Meaning:

            - This will appear after REBASE/CHECKOUT

            - Push will fail

        Solution:

            git checkout main
            
ERORS:

    1. Utracked files present

        Error message:

            Untracked file:

        Meaning:

            Git don't know about the file.

        Solution:

            git add <file>

        Memory hook:

            Untracked = add

    ------------------------------------------------------------------------

    2. FATAL : Not a git repository

        Error message:

            Fatal: not a git repository

        meaning:

            You're not inside the git repo.

        Solution:

            cd repo-folder

            OR

            git init

## CORE ERROR PROBLEM:

    Error message:
         
         non-fast forward / failed to push some refs / Diverged branches

    Meaning :

        - local and remote or not in same state.

    Visual: 

        Remote: A - B

        Local : A - C

        - Git is saying mismatch in history.

        - Visual clearly saying mismatch in remote and local.
    
    Our main goal in visual:

        Remote:

            A -B -C

        Local:

            A -B -C
        
        - Both should be in same line

    Solutions:

        1. Go to repo root

            Run:

                cd /workspaces/VK18-Linux

            Why?

            - Git commands is safest in repo root.

            Beacuse:
            
            - If not in repo root - some files will miss.

            - Relative path issue will come

            Memory hook:

                Repo root = safe git

        2. Stash

            Run:

                git stash

            Why?

            - local was uncommitted so we need to pull therefore need to do stash.

            Problem:

            - If working directory is dirty then git will not pull.

            What stash will do?

            - It will place it in temporary locker.

            Memoery hook:

                Before push - stasj=h shield

        3. Pull with rebase

            Run:

                git pull origin main --rebase

            Why?

            - It's main fix

            - Because remote was in AHEAD situation or diverged branches so.

            What rebas ewill do?

            - It rewrites the hotory cleanly.

            Before:

                Remote: A - B

                local: A - C

            After:

                Remote: A - B - C

                local: A - B - C

            Memory hook:

                History mismatch = do rebase

        4. Stash pop

            Run:

                git stash pop

            Why?

            - Whatever changes locked in stash for temporary purpose. Now we need to bring them back.

            - If you not do this then it will disappear so need to do pop.

            Memory hook:

            - Stash (temprory lock) = pop (release from lock)

        5. Add

            Run:

                git add .

            why?

            - Git commit only do for staged files.

            Memory hook:

            - Modify add --> Add first

        6. Commit

            Run:

                git commit -m "message"

            why?

            -To add local chnages into history.

        7. Push

            Run:

                git push

            why?

             - To algin both local and remote.

--

## PRO TIPS:

    Step1:

        git status

    Step2: Read the message

        If found:

            - Behind --> pull

            - Ahead  --> push

            - Diverged --> rebase+push

    PRO mantra :

        Check the status --> Take decision --> run commands


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

