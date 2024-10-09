# Help for Builtins
In this challenge, we learn about `builtins` which are kind of like commands built in the shell itself, and so we can directly call them without mentioning a directory. 
So we use the `help` command to get the secret value and then input that alongside the command to unlock the flag.
```
Connected!
hhacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "8TviNxMc".
hacker@man~help-for-builtins:~$ challenge --secret 8TviNxMc
Correct! Here is your flag!
pwn.college{8TviNxMcUrFZk4nWjaa_7XShIS5.dRTM5QDLzIzN0czW}
hacker@man~help-for-builtins:~$
```
