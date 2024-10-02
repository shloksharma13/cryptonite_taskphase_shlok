# Implicit Relative Path
In this module we learn that we cannot execute a direct program at the risk of executing programs in our current directory that have the same names as core system utilities.
Therefore we must use a relative path `./command` instead of `command`
```
Connected!
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{YVap6bcgEnEhhQFGTX3-huE9_CS.dFTN1QDLzIzN0czW}
hacker@paths~implicit-relative-path:/challenge$
```
