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


