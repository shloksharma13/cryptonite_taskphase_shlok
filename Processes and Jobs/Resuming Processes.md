# Resuming Processes
In this challenge, we learn how to use the `fg` builtin command to negate the effects of `Ctrl+Z` and basically resume a process that was interrupted by `Ctrl+Z`
```
Connected!
hacker@processes~resuming-processes:~$ /challenge/run
Let's practice resuming processes! Suspend me with Ctrl-Z, then resume me with
the 'fg' command! Or just press Enter to quit me!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~resuming-processes:~$ fg
/challenge/run
I'm back! Here's your flag:
pwn.college{QQfjPdAa4omytxqWxn8Jw8LlnGg.dZDN4QDLzIzN0czW}
Don't forget to press Enter to quit me!

Goodbye!
hacker@processes~resuming-processes:~$
```
