# Helpful Programs
In this challenge we learn to use the `--help` argument, we go through the help displayed and obtain the correct value and use it to unlock the flag.
```
hacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 39
hacker@man~helpful-programs:~$ /challenge/challenge -v
I'm exactly the version I need to be!
hacker@man~helpful-programs:~$ /challenge/challenge -g 39
Correct usage! Your flag: pwn.college{Aw_0RPT3CSlN9Z04Di9Fij7MF6S.ddjM4QDLzIzN0czW}
hacker@man~helpful-programs:~$
```
