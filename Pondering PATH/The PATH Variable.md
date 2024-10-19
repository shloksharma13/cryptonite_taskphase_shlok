# The PATH Variable
In this challenge, we learn what `PATH` is. It is basically the shell where directories are stored, so if we want to fool the command we just need to change the `PATH` and run it so that it cant find the delete command.
```
Connected!
hacker@path~the-path-variable:~$ PATH=""
hacker@path~the-path-variable:~$ /challenge/run
Trying to remove /flag...
/challenge/run: line 4: rm: No such file or directory
The flag is still there! I might as well give it to you!
pwn.college{Iu8BP2y7oGuduhUAARUPSQkDASM.dZzNwUDLzIzN0czW}
hacker@path~the-path-variable:~$
```
