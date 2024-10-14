# Exporting Variables
In this challenge we're learn that we can export the variable and its content by using the command `export` and to obtain the flag we're instructed to export a variable `PWN` with content `COLLEGE` and a non exported variable `COLLEGE` with content `PWN`. We do this and unlock the flag.
```
Connected!
hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ export PWN=COLLEGE
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ /challenge/run
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great
job! Here is your flag:
pwn.college{UmHx37NeJbEpPb9QM4KB21wwjfi.dJjN1QDLzIzN0czW}
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$
```
