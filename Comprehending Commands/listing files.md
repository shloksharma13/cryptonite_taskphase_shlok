# listing files
In this challenge, we're supposed to learn about `ls` command which enlists the files under a directory.
So we use `ls /challenge` to display the files under `/challenge` directory, which shows us the `run` file new name.
We then use `/challenge/23714-renamed-run-4840` to unlock the flag.
```
root@DESKTOP-BDBALR6:~# ssh -i ./key hacker@dojo.pwn.college
Connected!
hacker@commands~listing-files:~$ ls /challenge
23714-renamed-run-4840  DESCRIPTION.md
hacker@commands~listing-files:~$ /challenge/23714-renamed-run-4840
Yahaha, you found me! Here is your flag:
pwn.college{4mVJT2h-bN2nR_GuQ_XyJ7g8HWI.dhjM4QDLzIzN0czW}
hacker@commands~listing-files:~$
```
