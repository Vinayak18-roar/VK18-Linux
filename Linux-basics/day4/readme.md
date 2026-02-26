## Basic setup before going to start day4

### we created the day4 folder using mkdir

### we created practice file and readme files.

## Below basic steps we followed before the actual work.

**checking lists of current path**

@Vinayak18-roar ➜ /workspaces/VK18-Linux (main) $ ls

Linux-basics  Readme.md

**Print current working directory**

@Vinayak18-roar ➜ /workspaces/VK18-Linux (main) $ pwd

/workspaces/VK18-Linux

**Changing directory to my actual working location**

@Vinayak18-roar ➜ /workspaces/VK18-Linux (main) $ cd Linux-basics

**Change the directory to day4**

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics (main) $ cd day4

**Checking list in day4**

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ ls

practice_day4.txt  readme.md  testdir

--

**Removing existed testdir file using - rm**

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ rm -rf testdir

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ ls

practice_day4.txt  readme.md

---Successfully removed the existed folder from day4---

## Actual start for folders with mv command

**Now we are creating a file without using touch and creating along with contents in it**

**File.txt creation**

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ echo "Hi vinay" >> file.txt

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ ls

file.txt  practice_day4.txt  readme.md

**Multiple folders creation using mkdir**

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ mkdir dir dir1 testdir

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ ls

dir  dir1  file.txt  practice_day4.txt  readme.md  testdir

**checking lists of all directories**

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ ls

dir  dir1  file.txt  practice_day4.txt  readme.md  testdir

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ ls dir

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ ls dir1

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ ls testdir

**Note: Nothing listed in directories**
--
**checking contents inside file which we already created beofre**

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ cat file.txt

Hi vinay

## mv command starts from here:

### syntax: 

**mv sourcefile Destinationfile**

**Before moving file into folder checked the lists**

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ ls

dir  dir1  file.txt  practice_day4.txt  readme.md  testdir

**Moving file into folder**

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ mv file.txt dir

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ ls

dir  dir1  practice_day4.txt  readme.md  testdir

**file placed into folder**

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ ls dir

file.txt

-- Succesfully moved file into folder-----

### mv on folders

**Current lists checked here:**

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ ls

dir  dir1  practice_day4.txt  readme.md  testdir

**moving folder into another folder**

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ mv dir1 testdir

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ ls

dir  practice_day4.txt  readme.md  testdir

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ ls testdir

dir1

--Successfully moved dir1 folder into testdir folder--

**Now we are moving a folder which has a file in it : dir**

**Cheked list of dir:-**

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ ls dir

file.txt

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ mv dir testdir

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ ls

practice_day4.txt  readme.md  testdir

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ ls testdir

dir  dir1

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ ls testdir/dir

file.txt

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ ls

practice_day4.txt  readme.md  testdir

--Sucessfully moved the folder along with it's files**

## Renaming folder using mv command

### Condition : Folder will only rename when it's non-existing folder

**Check here praticed_folder is not existed before**

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ ls

practice_day4.txt  readme.md  testdir

**Here we used non-existing folder name : praticed_folder**

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ mv testdir praticed_folder

**checking by ls**

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ ls

practice_day4.txt  praticed_folder  readme.md

**Above testdir folder is renamed as praticed_folder**

**testdir renamed to praticed_folder and contents of testdir will not erase because it's in the place of source**

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day4 (main) $ ls praticed_folder

dir  dir1