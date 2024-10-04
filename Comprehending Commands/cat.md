# cat: not the pet, but the command!
In this challenge, we were supposed to read out the flag stored in `flag` file.
So we use the command `cat` with argument `flag` to read out the flag file and unlock the flag.
```
root@DESKTOP-BDBALR6:~# ssh -i ./key hacker@dojo.pwn.college
Connected!
hacker@commands~cat-not-the-pet-but-the-command:~$ cat flag
pwn.college{8Ws6lu1-S21lBTgJMWZ8LTkc4B_.dFzN1QDLzIzN0czW}
hacker@commands~cat-not-the-pet-but-the-command:~$
```
