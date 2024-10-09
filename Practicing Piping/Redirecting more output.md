# Redirecting more output
In this challenge, we shift the output of `/challenge/run` which is the flag to `myflag` by using `>`. 
And then we print `myflag` by using `cat` command.
```
hacker@piping~redirecting-more-output:~$ /challenge/run > myflag
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
cahacker@piping~redirecting-more-output:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{MUWkFi-EUoAHdYP7P9cZjVQJ-2W.dVjN1QDLzIzN0czW}

hacker@piping~redirecting-more-output:~$
```
