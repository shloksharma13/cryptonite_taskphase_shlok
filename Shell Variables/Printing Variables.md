# Printing Variables
In this challenge we learn about variables and how printing them requires usage of `$` sign as a prepend. To obtain the flag we were instructed to print the `FLAG` variable so we use `$FLAG` to print it.
```
root@DESKTOP-BDBALR6:~# ssh -i ./key hacker@dojo.pwn.college
Connected!
hacker@variables~printing-variables:~$ echo $FLAG
pwn.college{Asl2KeoZvYRVCNAhh9ejd_nwPCj.ddTN1QDLzIzN0czW}
hacker@variables~printing-variables:~$
```
