# Catting absolute paths
In this challenge we were supposed to access the flag from `/flag` directory and read it using the `cat` command.
Therefore we use `cat` with the argument `/flag` to read the file and unlock the flag.
```
Connected!
hacker@commands~catting-absolute-paths:~$ cd /flag
ssh-entrypoint: cd: /flag: Not a directory
hacker@commands~catting-absolute-paths:~$ cat /flag
pwn.college{wFqDec4X2rlCXZlQT30TgTG0qaM.dlTM5QDLzIzN0czW}
hacker@commands~catting-absolute-paths:~$
```
