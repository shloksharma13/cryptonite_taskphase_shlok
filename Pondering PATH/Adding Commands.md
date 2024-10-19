# Adding Commands
In this challenge, we first make a file win, and then edit it to run the command `cat /flag` when ran. Then we change the path to `../home/hacker` so that it can access `win` file which I `touch`ed there. Then we try running it but it doesnt work, so we change the permissions of `win` to executable and try again to unlock the flag.
```
Connected!
hacker@path~adding-commands:~$ touch win
hacker@path~adding-commands:~$ nano win
hacker@path~adding-commands:~$ echo PATH
PATH
hacker@path~adding-commands:~$ echo $PATH
/run/challenge/bin:/run/workspace/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
hacker@path~adding-commands:~$ PATH=$PATH:/home/hacker
hacker@path~adding-commands:~$ /challenge/run
Invoking 'win'....
/challenge/run: line 4: /home/hacker/win: Permission denied
It looks like that did not work... Did you set PATH correctly?
hacker@path~adding-commands:~$ echo $PATH
/run/challenge/bin:/run/workspace/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/home/hacker
hacker@path~adding-commands:~$ chmod a+x win
hacker@path~adding-commands:~$ /challenge/run
Invoking 'win'....
pwn.college{8-jJzCNQEb4epLZsZ9rB_o-O1vD.dZzNyUDLzIzN0czW}
hacker@path~adding-commands:~$
```
