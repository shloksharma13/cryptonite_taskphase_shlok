# Intro to commands
We link our ubuntu to pwn.college, once its connected we use the commands ```whoami``` which gives us the name of the user viz. ```hacker``` for this case
Then we invoke the command ```hello``` which prints success and gives us our flag.
```
root@DESKTOP-BDBALR6:~# ssh -i ./key hacker@dojo.pwn.college
Connected!
hacker@hello~intro-to-commands:~$ whoami
hacker
hacker@hello~intro-to-commands:~$ hello
Success! Here is your flag:
pwn.college{olzC2196rfMFGCQo6tXmpY22ETB.ddjNyUDLzIzN0czW}
hacker@hello~intro-to-commands:~$
```
