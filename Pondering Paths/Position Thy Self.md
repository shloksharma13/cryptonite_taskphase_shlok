# Position Thy Self
In this module we learn how to change directories.
The challenge was to invoke `challenge/run` but once we ran it, the parses prompts that we're in the wrong directory and informs us where to run the challenge.
Thus we use `cd /usr/share/doc` to change our root directory to the necessary directory.
Here we learn that instead of having the programs stored in the root directory we can have them under others and access them by changing the directory when needed.
Once we're in `/usr/share/doc` we invoke the command `/challenge/run` to achieve success and unlock the flag.
```
Connected!
hacker@paths~position-thy-self:~$ /challenge/run
Incorrect...
You are not currently in the /usr/share/doc directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:~$ cd /usr/share/doc
hacker@paths~position-thy-self:/usr/share/doc$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{o3JTD3tRRaPZ92quBLr3TblhC2P.dZDN1QDLzIzN0czW}
hacker@paths~position-thy-self:/usr/share/doc$
```
