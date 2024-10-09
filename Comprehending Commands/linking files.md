# linking files
In this challenge we learn to use the command `ln` with the argument `s`. From what I learnt, `ln` is a linking command and `-s` argument signifies a symbolic command.
Therefore we first link `/flag` with `~/not-the-flag` and run the challenge to unlock the flag.
```
root@DESKTOP-BDBALR6:~# ssh -i ./key hacker@dojo.pwn.college
Connected!
hacker@commands~linking-files:~$ ln -s /flag ~/not-the-flag
hacker@commands~linking-files:~$ /challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{EOFEsvTqsPomF7Ohx1fp8tFPFFU.dlTM1UDLzIzN0czW}
hacker@commands~linking-files:~$
```
