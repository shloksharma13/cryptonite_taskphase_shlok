# Position Elsewhere
This is a repition of the previous module, most likely for practice.
In this module we are required to run `/challenge/run` but when we run it  in the root directory it shows that the program is residing in `/sys/kernel` directory.
So we use `cd /sys/kernel` to change our current directory and run `/challenge/run` in that directory to achieve success and unlock the flag.
```
Connected!
hacker@paths~position-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /sys/kernel directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:~$ cd /sys/kernel
hacker@paths~position-elsewhere:/sys/kernel$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{4J_bqF3TcevSOtbwWESTB8JfmOB.ddDN1QDLzIzN0czW}
hacker@paths~position-elsewhere:/sys/kernel$
```
