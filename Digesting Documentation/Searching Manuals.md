# Searching Manuals
In this challenge we learn about searching a manual using the `/` and the `?` commands for searchign forward and backward respectively.
Thus we read the manual by using `man challenge` and then use `/flag` to find the argument that unlocks the flag.
```
Connected!
hacker@man~searching-manuals:~$ man challenge
hacker@man~searching-manuals:~$ man challenge
hacker@man~searching-manuals:~$ /challenge --wnhze
ssh-entrypoint: /challenge: Is a directory
hacker@man~searching-manuals:~$ /challenge/challenge --wnhze
Initializing...
Correct usage! Your flag: pwn.college{gJAaKS7_usszemP5YXSxgrFafXk.dVTM4QDLzIzN0czW}
hacker@man~searching-manuals:~$
```
