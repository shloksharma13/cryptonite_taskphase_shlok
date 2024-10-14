# Storing Command Output
In this challenge we learn how we can directly store an output into a variable by using `$()`.
```
ker@variables~storing-command-output:~$ PWN=$(/challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out
and submit it!
hacker@variables~storing-command-output:~$ echo "$PWN"
pwn.college{Qgs3fkiOtvtih80WjeyUSqXtMhf.dVzN0UDLzIzN0czW}
hacker@variables~storing-command-output:~$
```
