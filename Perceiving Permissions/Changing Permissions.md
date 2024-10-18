# Changing Permissions
In this challenge, we learn that we can change a file's permissions to read and write etc. The most notable thing in my opninion is that `+` represents adding permissions and `-` represents removing permisssion.
```
Connected!
hacker@permissions~changing-permissions:~$ ls -l
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
hacker@permissions~changing-permissions:~$ chmod go+rwx /flag
hacker@permissions~changing-permissions:~$ cat /flag
pwn.college{Uj1Qk4w36ooPINtb_NtabWB0fDS.dNzNyUDLzIzN0czW}
hacker@permissions~changing-permissions:~$
```
