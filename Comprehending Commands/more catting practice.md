# more catting practice
In this challenge, we're given the directory to the flag which is `/usr/lib/sas12/flag`, so we use the `cat` command to read it.
Therefore we input `cat /usr/lib/sas12/flag` to the parser to unlock the flag.
```
Connected!
You cannot use the 'cd' command in this level, and must retrieve the flag by
absolute path. Plus, I hid the flag in a different directory! You can find it
in the file /usr/lib/sasl2/flag. Go cat it out **without** cding into that
directory!
hacker@commands~more-catting-practice:~$ cat /usr/lib/sasl2/flag
pwn.college{EqR7wenPbRxNVBfPyRzFNnIs7Wn.dBjM5QDLzIzN0czW}
hacker@commands~more-catting-practice:~$
```
