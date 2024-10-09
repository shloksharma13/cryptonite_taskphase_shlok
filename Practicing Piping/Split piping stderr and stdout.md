# split piping stderr and stdout
In this challenge we run the command and redirect its output to `planet` and error to `the` which are programs so we enclose them in parenthesis.
```
Connected!
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack > >(/challenge/planet) 2> >(/challenge/the)
Congratulations, you have learned a redirection technique that even experts
struggle with! Here is your flag:
pwn.college{4_CQ6b3qAAEc43qwq6WAOWTFeUS.dFDNwYDLzIzN0czW}
hacker@piping~split-piping-stderr-and-stdout:~$
```
