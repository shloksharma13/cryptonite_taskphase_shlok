# Exclusionary Globs
In this challenge, we learn to write globs that dont include certain elements, for that we use `! or ^` in the argument.
```
Connected!
hacker@globbing~exclusionary-globbing:~$ /challenge/run /challenge/files/[^pwn]*
Error: please run with a working directory of /challenge/files!
hacker@globbing~exclusionary-globbing:~$ cd /challenge/files
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [^pwn]*
You got it! Here is your flag!
pwn.college{whjKAFjWPCnRfDaYYwXFGnIhYEK.dZjM4QDLzIzN0czW}
hacker@globbing~exclusionary-globbing:/challenge/files$
```
