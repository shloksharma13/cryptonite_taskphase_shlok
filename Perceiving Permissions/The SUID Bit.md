# The SUID Bit 
In this challenge, we use `chmod` with `u+s` argument to add the SUID Bit to the program, then run it and `cat` the flag.
```
hacker@permissions~the-suid-bit:~$ chmod u+s /challenge/getroot
hacker@permissions~the-suid-bit:~$ /challenge/getroot
SUCCESS! You have set the suid bit on this program, and it is running as root!
Here is your shell...
root@permissions~the-suid-bit:~# cat /flag
pwn.college{466KvYQQNeZwqO9oVsS_3-4mVAZ.dNTM2QDLzIzN0czW}
root@permissions~the-suid-bit:~#
```
