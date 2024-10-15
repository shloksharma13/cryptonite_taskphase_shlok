# Suspending Processes
In this challenge, we learn how to use the `Ctrl+Z` to suspend a command while its being run.
```
Connected!
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root          82      65  0 17:14 pts/0    00:00:00 bash /challenge/run
root          84      82  0 17:14 pts/0    00:00:00 ps -f

I don't see a second me!

To pass this level, you need to suspend me and launch me again! You can
background me with Ctrl-Z or, if you're not ready to do that for whatever
reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root          82      65  0 17:14 pts/0    00:00:00 bash /challenge/run
root          89      65  0 17:14 pts/0    00:00:00 bash /challenge/run
root          91      89  0 17:14 pts/0    00:00:00 ps -f

Yay, I found another version of me! Here is the flag:
pwn.college{Mv0Tn97NJD6PRScSBbXiR_dniXK.dVDN4QDLzIzN0czW}
hacker@processes~suspending-processes:~$
```
