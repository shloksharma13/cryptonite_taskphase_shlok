# Reading Manuals
In this challenge, we learn about reading manuals, we use the command `man` with the argument `challenge` to read the manual of `challenge`.
We read the manual to uncover how to unlock the flag and use the necessary command and arguments.
```
Connected!
mahacker@man~reading-manuals:~$ man challenge

CHALLENGE(1)                                                   Challenge Commands                                                   CHALLENGE(1)

NAME
       /challenge/challenge - print the flag!

SYNOPSIS
       challenge OPTION

DESCRIPTION
       Output the flag when called with the right arguments.

       --fortune
              read a fortune

       --version
              output version information and exit

       --szlbwf NUM
              print the flag if NUM is 844

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The repository for this dojo: <https://github.com/pwncollege/linux-luminarium/>

SEE ALSO
       man(1) bash-builtins(7)

pwn.college                                                         May 2024                                                        CHALLENGE(1)
hacker@man~reading-manuals:~$ /challenge/challenge --szlbwf 844
Correct usage! Your flag: pwn.college{szlbwGfmgY8pVbT4NPIYVJAUNCE.dRTM4QDLzIzN0czW}
hacker@man~reading-manuals:~$
```
