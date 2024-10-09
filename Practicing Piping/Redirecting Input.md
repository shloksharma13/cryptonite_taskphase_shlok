# Redirecting Input
In this challenge we learn to input the contents of a file into a command. 
We first redirect the output of `COLLEGE` to `PWN` using `>` and then use that to input into `/challenge/run` using `<`.
```
Connected!
hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{op2706Mn0kW7NgiNMF-McRKLmZw.dBzN1QDLzIzN0czW}
hacker@piping~redirecting-input:~$
```
