# removing files
In this challenge, we learn how to use the `rm` command to delete files.
We start by checking the files present in the home directory by the command `ls`. Then we use the command `rm` with the argument `delete_me` to delete the file.
Then we run the code `challenge/check` to unlock the flag.
```
Connected!
hacker@commands~removing-files:~$ ls
Desktop  a  delete_me
hacker@commands~removing-files:~$ rm delete_me
hacker@commands~removing-files:~$ ls
Desktop  a
hacker@commands~removing-files:~$ /challenge/check
Excellent removal. Here is your reward:
pwn.college{Auz6AOqNqNzuX_XbRQkSFUkxCu2.dZTOwUDLzIzN0czW}
hacker@commands~removing-files:~$
```
