# Position Yet Elsewhere
This is yet again a repition of the previous module where we run the command, get an error, fix the directory, and run it again to achieve success and unlock the flag.
```
Connected!
hacker@paths~position-yet-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /sys directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:~$ cd /sys
hacker@paths~position-yet-elsewhere:/sys$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{wnsOELQVtqqwKTTBJkCaj2xH0R9.dhDN1QDLzIzN0czW}
hacker@paths~position-yet-elsewhere:/sys$
```
