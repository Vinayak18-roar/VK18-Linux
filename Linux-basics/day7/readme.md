@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day7 (main) $ mkdir dir/dir1
mkdir: cannot create directory ‘dir/dir1’: No such file or directory
@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day7 (main) $ mkdir dir
@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day7 (main) $ mkdir -p dir/dir1
@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day7 (main) $ ls
dir  pratice.txt  readme.md
@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day7 (main) $ ls dir
dir1
@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day7 (main) $ cd dir
@Vinayak18-roar ➜ .../VK18-Linux/Linux-basics/day7/dir (main) $ ln -s . loop
@Vinayak18-roar ➜ .../VK18-Linux/Linux-basics/day7/dir (main) $ ls loop
@Vinayak18-roar ➜ .../VK18-Linux/Linux-basics/day7/dir (main) $ cd loop
@Vinayak18-roar ➜ .../Linux-basics/day7/dir/loop (main) $ pwd
/workspaces/VK18-Linux/Linux-basics/day7/dir/loop
@Vinayak18-roar ➜ .../Linux-basics/day7/dir/loop (main) $ cd loop
@Vinayak18-roar ➜ .../day7/dir/loop/loop (main) $ pwd
/workspaces/VK18-Linux/Linux-basics/day7/dir/loop/loop
@Vinayak18-roar ➜ .../day7/dir/loop/loop (main) $ cd ..
@Vinayak18-roar ➜ .../Linux-basics/day7/dir/loop (main) $ cd ..
@Vinayak18-roar ➜ .../VK18-Linux/Linux-basics/day7/dir (main) $ cd ..



@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day7 (main) $ mkdir a
@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day7 (main) $ mkdir b
@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day7 (main) $ ls
a  b  dir  pratice.txt  readme.md
@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day7 (main) $ ls -r
readme.md  pratice.txt  dir  b  a
@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day7 (main) $ ls -t
b  a  dir  readme.md  pratice.txt
@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day7 (main) $ ls -R
.:
a  b  dir  pratice.txt  readme.md

./a:

./b:

./dir:
dir1  loop

./dir/dir1:
@Vinayak18-roar ➜ /workspaces/VK18-Linux/Linux-basics/day7 (main) $ ls -latR
.:
total 24
drwxrwxrwx+ 5 codespace codespace 4096 Mar  3 18:11 .
drwxrwxrwx+ 2 codespace codespace 4096 Mar  3 18:11 b
drwxrwxrwx+ 2 codespace codespace 4096 Mar  3 18:11 a
drwxrwxrwx+ 3 codespace codespace 4096 Mar  3 18:09 dir
-rw-rw-rw-  1 codespace codespace    0 Mar  2 18:27 readme.md
-rw-rw-rw-  1 codespace codespace   16 Mar  2 18:27 pratice.txt
drwxrwxrwx+ 9 codespace codespace 4096 Mar  2 18:26 ..

./b:
total 8
drwxrwxrwx+ 2 codespace codespace 4096 Mar  3 18:11 .
drwxrwxrwx+ 5 codespace codespace 4096 Mar  3 18:11 ..

./a:
total 8
drwxrwxrwx+ 5 codespace codespace 4096 Mar  3 18:11 ..
drwxrwxrwx+ 2 codespace codespace 4096 Mar  3 18:11 .

./dir:
total 12
drwxrwxrwx+ 5 codespace codespace 4096 Mar  3 18:11 ..
drwxrwxrwx+ 3 codespace codespace 4096 Mar  3 18:09 .
lrwxrwxrwx  1 codespace codespace    1 Mar  3 18:09 loop -> .
drwxrwxrwx+ 2 codespace codespace 4096 Mar  3 18:08 dir1

./dir/dir1:
total 8
drwxrwxrwx+ 3 codespace codespace 4096 Mar  3 18:09 ..
drwxrwxrwx+ 2 codespace codespace 4096 Mar  3 18:08 .