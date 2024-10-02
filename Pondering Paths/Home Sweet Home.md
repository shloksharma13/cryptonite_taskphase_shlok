# Home Sweet Home
In this challenge we learn about home directory and how `~` referes to the home.
Say a user `xyz` inputs into the parser `echo ~` the output would be `/home/xyz` because that's the home directory for the user.
Now in this challenge we're supposed to run a challenge while giving a three letter argument that must be in the home directory
Therefore we use `~` to refer to home and `/` to refer to files under home, and `a` to refer to the file we assume is a.
Thus the argument to the command `run` is `~/a`
This unlocks the flag.
```
Connected!
hacker@paths~home-sweet-home:~$ /challenge/run ~/a
Writing the file to /home/hacker/a!
... and reading it back to you:
pwn.college{gwukMTOE5q4ixRs9Y9ZswJJtYtr.dNzM4QDLzIzN0czW}
hacker@paths~home-sweet-home:~$
```
