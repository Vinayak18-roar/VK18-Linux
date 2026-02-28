## INODE

Every file on a Linux system has an **inode** which is also referred
to as **index node**

- An inode is basically a file structure. It's a database which contains all of a file information except two things , **namely file contents** and **file name**.

- Typically an inode contains the following information about a
file

(1) Inode number
(2) File size
(3) File type
(4) Owner
(5) Permissions
(6) Number of Links

- Let's say we have a file called file.txt, If you want to view the inode
number of file.txt

Then you just type **ls i file1.txt**

- And so typing **ls i** will show allthe inode numbers in your current directory

### Example:

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day5 (main) $ ls -il

1573229 drwxrwxrwx+ 2 codespace codespace 4096 Feb 28 18:22 dir

1573222 -rw-rw-rw-  2 codespace codespace    0 Feb 28 18:22 file.txt

--

## HARD LINK  & SOFT LINK

@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day5 (main) $ ls
practice.txt  readme.md
@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day5 (main) $ touch file.txt
@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day5 (main) $ mkdir dir
@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day5 (main) $ ls
dir  file.txt  practice.txt  readme.md
@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day5 (main) $ ls -i
1573229 dir  1573222 file.txt  1573163 practice.txt  1573223 readme.md