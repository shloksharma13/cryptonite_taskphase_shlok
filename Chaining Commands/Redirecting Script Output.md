# Redirecting Script Output
In this challenge, we use the same `x.sh` file since it has the commands we need to use, then we use our piping techniques to pipe the output of `bash x.sh` directly into the required command.
```
Connected!
hacker@chaining~redirecting-script-output:~$ touch x.sh
hacker@chaining~redirecting-script-output:~$ nano x.sh
hacker@chaining~redirecting-script-output:~$ bash x.sh | /challenge/solve
Correct! Here is your flag:
pwn.college{cPzWPH5aRLI0hOpiHvn2B65WuF3.dhTM5QDLzIzN0czW}
hacker@chaining~redirecting-script-output:~$ C
```
