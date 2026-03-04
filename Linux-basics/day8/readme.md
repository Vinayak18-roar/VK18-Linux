labex:project/ $ ls

labex:project/ $ pwd

/home/labex/project

labex:project/ $ cd ~

labex:~/ $ pwd

/home/labex

labex:~/ $ ls

Code  Desktop  golang  project

labex:~/ $ echo ~

/home/labex

labex:~/ $ ls code

ls: cannot access 'code': No such file or directory

labex:~/ $ ls Code

labex:~/ $ ls Desktop

code.desktop  gedit.desktop  gvim.desktop  xfce4-terminal.desktop

labex:~/ $ cd ~/Project

cd: no such file or directory: /home/labex/Project

labex:~/ $ cd ~/project

labex:project/ $ cd ~/Desktop

labex:Desktop/ $ ls

code.desktop  gedit.desktop  gvim.desktop  xfce4-terminal.desktop

labex:Desktop/ $ cp ~/code .

cp: cannot stat '/home/labex/code': No such file or directory

labex:Desktop/ $ cd -    

~/project
labex:project/ $ cd -
~/Desktop
labex:Desktop/ $ cd ~
labex:~/ $ ls
Code  Desktop  golang  project
labex:~/ $ ls -F
Code/  Desktop/  golang/  project/
labex:~/ $ cp -r Code Desktop
labex:~/ $ ls
Code  Desktop  golang  project
labex:~/ $ cd ~
labex:~/ $ cd -
~
labex:~/ $ cd ~/Desktop
labex:Desktop/ $ ls
Code  code.desktop  gedit.desktop  gvim.desktop  xfce4-terminal.desktop
labex:Desktop/ $ cd -        
~
labex:~/ $ ls
Code  Desktop  golang  project
labex:~/ $ ls -a
.             .gdb_printer   project
..            .gemrc         .tmux.conf
.bash_logout  .gnupg         .vimrc
.bashrc       golang         .vnc
.cache        .ICEauthority  .Xauthority
Code          .kasmpasswd    .xscreensaver
.codeblocks   .local         .zcompdump
.config       .npm           .zcompdump-69a81c128a8ad61e36d16188-5.8.1
.dbus         .oh-my-zsh     .zcompdump-buildkitsandbox-5.8.1
Desktop       .pip           .zsh_history
.gdbinit      .profile       .zshrc
labex:~/ $ cp .zhrc ~/Desktop/zhrc-copy
cp: cannot stat '.zhrc': No such file or directory
labex:~/ $ cp .zshrc ~/Desktop/zshrc-copy
labex:~/ $ ls
Code  Desktop  golang  project
labex:~/ $ ls -a
.             .gdb_printer   project
..            .gemrc         .tmux.conf
.bash_logout  .gnupg         .vimrc
.bashrc       golang         .vnc
.cache        .ICEauthority  .Xauthority
Code          .kasmpasswd    .xscreensaver
.codeblocks   .local         .zcompdump
.config       .npm           .zcompdump-69a81c128a8ad61e36d16188-5.8.1
.dbus         .oh-my-zsh     .zcompdump-buildkitsandbox-5.8.1
Desktop       .pip           .zsh_history
.gdbinit      .profile       .zshrc
labex:~/ $ cd -
~/Desktop
labex:Desktop/ $ ls
Code          gedit.desktop  xfce4-terminal.desktop
code.desktop  gvim.desktop   zshrc-copy
labex:Desktop/ $ 
labex:Desktop/ $ 
labex:Desktop/ $ 
