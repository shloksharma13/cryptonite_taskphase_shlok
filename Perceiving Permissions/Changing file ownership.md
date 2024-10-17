# Changing File Ownership
In this challenge, we proceed by printing out a list of the directory using `ls -l` allowing us to see the files. Then we use `chown` command with the arguments `hacker` and `/flag` since we wish to change the owner of `/flag` to `hacker`.
This gets us the required permission to read `/flag` using `cat`.
```
Connected!
hacker@permissions~changing-file-ownership:~$ ls -l
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
hacker@permissions~changing-file-ownership:~$ chown hacker /flag
hacker@permissions~changing-file-ownership:~$ cat /flag
pwn.college{wwjdPwn8SUruAW3OrfXGi9FXpvA.dFTM2QDLzIzN0czW}
hacker@permissions~changing-file-ownership:~$
```
