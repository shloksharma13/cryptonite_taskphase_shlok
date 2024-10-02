In this module we learn about arguments
The first word we input in the prompt is the command, and the subsequent words are arguments
In this case ```echo``` was a command with ```Hello Hackers!``` as the argument
Thus when the parses read ```echo``` it echoes the argument.
The challenge was to run the command ```hello``` with the argument ```hacker```
Thus our input to the parser is ```hello hackers```
This gives success to the challenge and gets us the flag!
```
Connected!
hacker@hello~intro-to-arguments:~$ echo Hello Hackers!
Hello Hackers!
hacker@hello~intro-to-arguments:~$ hello hackers
Success! Here is your flag:
pwn.college{QCcXq3-i4wwRrARqoEvs6P4rTCd.dhjNyUDLzIzN0czW}
hacker@hello~intro-to-arguments:~$
```
