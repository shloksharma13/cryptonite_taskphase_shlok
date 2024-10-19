# Executable Shell Scripts
In this challenge, we start by making a shell script named `y.sh` and then change its permissions to make it executable, and then we run it without explicitly calling `bash`.
```
root@DESKTOP-BDBALR6:~# ssh -i ./key hacker@dojo.pwn.college
Connected!
hacker@chaining~executable-shell-scripts:~$ touch y.sh
hacker@chaining~executable-shell-scripts:~$ nano y.sh
hacker@chaining~executable-shell-scripts:~$ ls -l
total 8988
-rw-r--r-- 1 hacker hacker        4 Oct  9 12:54 COLLEGE
drwxr-xr-x 2 hacker hacker     4096 Sep 30 20:37 Desktop
-rw-r--r-- 1 hacker hacker      233 Oct 14 20:31 PWN
-rw-r--r-- 1 root   hacker       58 Oct  2 20:12 a
-rw-r--r-- 1 root   hacker       77 Oct  9 18:07 college
-rw------- 1 hacker hacker 35045376 Oct 19 17:08 core
-rw-r--r-- 1 hacker hacker      829 Oct  9 14:54 instructions
-rw-r--r-- 1 root   hacker       77 Oct  9 18:20 intercept
-rw-r--r-- 1 hacker hacker        0 Oct  9 13:09 myfile
-rw-r--r-- 1 root   hacker       93 Oct  9 14:54 myflag
lrwxrwxrwx 1 hacker hacker        5 Oct  9 03:06 not-the-flag -> /flag
-rw-r--r-- 1 root   hacker       77 Oct  9 18:08 pwn
-rw-r--r-- 1 hacker hacker        0 Oct 19 17:10 pwn.sh
-rw-r--r-- 1 root   hacker       77 Oct  9 18:07 pwn_output
-rw-r--r-- 1 root   hacker      435 Oct  9 13:35 the-flag
-rw-r--r-- 1 hacker hacker       34 Oct 19 17:25 x.sh
-rw-r--r-- 1 hacker hacker       17 Oct 19 17:30 y.sh
hacker@chaining~executable-shell-scripts:~$ chmod a+x y.sh
hacker@chaining~executable-shell-scripts:~$ ./y.sh
Congratulations on your shell script execution! Your flag:
pwn.college{AdNhSDG_T8oZSM6SkapV0qQloG6.dRzNyUDLzIzN0czW}
hacker@chaining~executable-shell-scripts:~$
```
