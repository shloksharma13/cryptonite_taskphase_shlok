# Executable Files
In this challenge, we run the command `chmod a+x` to make the command `/challenge/run` accessible to all and then run it.
```
root@DESKTOP-BDBALR6:~# ssh -i ./key hacker@dojo.pwn.college
Connected!
hacker@permissions~executable-files:~$ chmod a+x /challenge/run
hacker@permissions~executable-files:~$ /challenge/run
Successful execution! Here is your flag:
pwn.college{sTkuFvzytc6cLvO-P_oko90vewG.dJTM2QDLzIzN0czW}
hacker@permissions~executable-files:~$
```
