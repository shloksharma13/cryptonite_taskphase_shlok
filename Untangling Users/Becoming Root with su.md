# Becoming Root with su
In this challenge, we prompt the parser with `su` command to switch the user from `hacker` to `root` and then enter the password which was provided to us. This makes us `root` and allows us to read the flag.
```
Connected!
hacker@users~becoming-root-with-su:~$ su
Password:
root@users~becoming-root-with-su:/home/hacker# cat /flag
pwn.college{g60jtPJ27S0OhErXseiJ0nM7wMF.dVTN0UDLzIzN0czW}
root@users~becoming-root-with-su:/home/hacker#
```
