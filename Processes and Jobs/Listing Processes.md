# Listing Processes
In this challenge we learn that by using the `ps -ef` and `ps aux` commands we can print down a list of commands that are currently running and details like the start time etc.
When we print out the running programs we spot the `/challenge` command with the modified `/run` command so we use that and unlock the flag.
```
root@DESKTOP-BDBALR6:~# ssh -i ./key hacker@dojo.pwn.college
Connected!
hacker@processes~listing-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 16:51 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/default/bin/dojo-init /ru
root           7       1  0 16:51 ?        00:00:00 /run/dojo/bin/sleep 6h
root          68       1  0 16:51 ?        00:00:00 /challenge/11969-run-9111
root          72      68  0 16:51 ?        00:00:00 sleep 6h
hacker        73       0  0 16:52 pts/0    00:00:00 /run/dojo/bin/ssh-entrypoint
hacker        90      73  0 16:52 pts/0    00:00:00 ps -ef
hacker@processes~listing-processes:~$ /challenge/11969-run-9111
Yahaha, you found me! Here is your flag:
pwn.college{4940MXYZSnjQtKyYVoYqcXkgj8V.dhzM4QDLzIzN0czW}
Now I will sleep for a while (so that you could find me with 'ps').
```
