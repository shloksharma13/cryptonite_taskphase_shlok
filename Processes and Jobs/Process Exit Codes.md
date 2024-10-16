# Process exit codes
In this challenge we learn how to use the `&?` function to get an exit code. We simultaneously use echo to print it out too. This gets us the exit code for the latest command ran.
```
Connected!
/hacker@processes~process-exit-codes:~$
hacker@processes~process-exit-codes:~$ /challenge/get-code
Exiting with an error code!
hacker@processes~process-exit-codes:~$ $?
ssh-entrypoint: 101: command not found
hacker@processes~process-exit-codes:~$ echo $?
127
hacker@processes~process-exit-codes:~$ /challenge/submit-code 127
Incorrect... Make sure to use $? immediately after running /challenge/get-code.
Your shell will overwrite the $? variable with the exit value of any other
command you run!
hacker@processes~process-exit-codes:~$ /challenge/get-code
Exiting with an error code!
hacker@processes~process-exit-codes:~$ echo $?
116
hacker@processes~process-exit-codes:~$ /challenge/submit-code 116
CORRECT! Here is your flag:
pwn.college{wLeZLGDjA0lS9cZOOY1aEriJxgu.dljN4UDLzIzN0czW}
hacker@processes~process-exit-codes:~$
```
