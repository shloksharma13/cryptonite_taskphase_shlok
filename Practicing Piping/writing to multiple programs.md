# Writing to multiple programs
In this challenge, we run the command to redirect the output of into planet and the by piping.
```
Connected!
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | tee >(/challenge/the) >(/challenge/planet)
This secret data must directly and simultaneously make it to /challenge/the and
/challenge/planet. Don't try to copy-paste it; it changes too fast.
25758311713261730959
Congratulations, you have duplicated data into the input of two programs! Here
is your flag:
pwn.college{Uw8Eun7_FEQJEuV5Zb8COzB8aId.dBDO0UDLzIzN0czW}
hacker@piping~writing-to-multiple-programs:~$
```
