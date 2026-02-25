## Change the directory using cd
- I have made folders inside **Linux-basics**.

@Vinayak18-roar ➜ /workspaces/VK18-Linux (main) $ cd Linux-basics

ls: list check before creating any folders or files.

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics (main) $ ls

day1  day2

- Creating folder for day3 using mkdir.

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics (main) $ mkdir day3

- Verfiying whether folder is created or not by ls.

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics (main) $ ls

day1  day2  day3

- Chnaging directory to day3

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics (main) $ cd day3

-Verifying any files or folders inside day3.(Not yet created).

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ ls

## Creating multiple files using **touch** command.

### Examples
Creating practice and readme files.

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ touch practice.txt readme.md

PWD: print working directory

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ pwd

/workspaces/VK18-Linux/Linux-basics/day3

- Verifying using ls.

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ ls

practice.txt  readme.md

- List in long formates:

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ ls -l

total 0
-rw-rw-rw- 1 codespace codespace 0 Feb 24 12:44 practice.txt
-rw-rw-rw- 1 codespace codespace 0 Feb 24 12:44 readme.md

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ ls -lh

total 0
-rw-rw-rw- 1 codespace codespace 0 Feb 24 12:44 practice.txt
-rw-rw-rw- 1 codespace codespace 0 Feb 24 12:44 readme.md

## Creating multiple files.

To pratcie created some files and verified by ls:

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ touch file.txt file1.txt file2.txt

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ ls

file.txt  file1.txt  file2.txt  practice.txt  readme.md

## Storing contents inside files.

By using **echo** command we can store contents in files.

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ echo "Hi, I'm from file.txt" >>file.txt

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ echo "Hi, I'm from file1.txt" 
>>file1.txt

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ echo "Hi, I'm from file2.txt" >>file2.txt

## Checking the contents of files using **cat** command.

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ cat file.txt

Hi, I'm from file.txt

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ cat file1.txt

Hi, I'm from file1.txt

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ cat file2.txt

Hi, I'm from file2.txt

## mv command:

### syntax
mv sourcefile destinationfile

mv command used basically for move/rename the files and folders.

## condition 1: mv on both existing files and non-empty files.

1: file.txt - sourcefile
   file1.txt - Destinationfile

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ mv file.txt file1.txt

Verify by ls.

Here file.txt renamed by file1.txt

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ ls

file1.txt  file2.txt  practice.txt  readme.md

Now checking contents of file1.txt. It has file.txt contents.

Note that -sourcefile content will not erase only file name will rename by destinationfile.

And file.txt overwrite the contents of file1.txt
                    OR
file1.txt content overwritten by file.txt

**Remember**: Whenever using mv on files sourcefile name only change(rename) to destinationfile. And erase the contents of destinationfile.

- Sourcefile content unchanged. if we check **file1.txt** content will see **file.txt** contents check below:

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ cat file1.txt

Hi, I'm from file.txt

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ mv file2.txt file1.txt

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ ls

file1.txt  practice.txt  readme.md

- Now **file1.txt** contents overwritten by **file2.txt** contents.
  
@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ cat file1.txt

Hi, I'm from file2.txt

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ ls

file1.txt  practice.txt  readme.md

- Now bring back to **file.txt**. But notice here currently **file.txt** is non-existing file.
  
- If existing or non existing file will be rename.
  
@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ mv file1.txt file.txt

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ ls

file.txt  practice.txt  readme.md

- file1 has file2 contents so that will be visible in file.

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day3 (main) $ cat file.txt

Hi, I'm from file2.txt
