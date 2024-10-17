# Groups and files
In this challenge we learn how to edit the author or the owner of a group which contains several files, once you own the group you get access to all the files in the group. So we first `ls` to find the command and then change its group's owner to `hacker` by using `chgrp`.
```
Connected!
hacker@permissions~groups-and-files:~$ ls -l
total 44
-rw-r--r-- 1 hacker hacker    4 Oct  9 12:54 COLLEGE
drwxr-xr-x 2 hacker hacker 4096 Sep 30 20:37 Desktop
-rw-r--r-- 1 hacker hacker  233 Oct 14 20:31 PWN
-rw-r--r-- 1 root   hacker   58 Oct  2 20:12 a
-rw-r--r-- 1 root   hacker   77 Oct  9 18:07 college
-rw-r--r-- 1 hacker hacker  829 Oct  9 14:54 instructions
-rw-r--r-- 1 root   hacker   77 Oct  9 18:20 intercept
-rw-r--r-- 1 hacker hacker    0 Oct  9 13:09 myfile
-rw-r--r-- 1 root   hacker   93 Oct  9 14:54 myflag
lrwxrwxrwx 1 hacker hacker    5 Oct  9 03:06 not-the-flag -> /flag
-rw-r--r-- 1 root   hacker   77 Oct  9 18:08 pwn
-rw-r--r-- 1 root   hacker   77 Oct  9 18:07 pwn_output
-rw-r--r-- 1 root   hacker  435 Oct  9 13:35 the-flag
hacker@permissions~groups-and-files:~$ chgrp hacker /flag
hacker@permissions~groups-and-files:~$ cat /flag
pwn.college{4oFVj5ZJxFLfpzgKVMF95suVCVx.dFzNyUDLzIzN0czW}
hacker@permissions~groups-and-files:~$
```
