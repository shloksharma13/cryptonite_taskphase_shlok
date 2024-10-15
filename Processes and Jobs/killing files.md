# Killing Files
In this challenge, we learn how to kill an ongoing process, we start by using `ps aux` to display all currently running processes and then find the id for `cont_run` and use the `kill` command with argument `73` which is the id for `dont_run` and kill it. then we run `/challenge/run` to unlcok the flag.
```
Connected!
hacker@processes~killing-processes:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.1  0.0   1056   640 ?        Ss   16:57   0:00 /sbin/docker-init -- /nix/var/nix/profiles/default/bi
root           7  0.0  0.0   5052  2240 ?        S    16:57   0:00 /run/dojo/bin/sleep 6h
root          71  0.0  0.0   4732  2880 ?        S    16:57   0:00 su -c /challenge/.launcher hacker
hacker        73  0.0  0.0   4976  3200 ?        Ss   16:57   0:00 /challenge/dont_run
hacker        74  0.0  0.0   5052  2560 ?        S    16:57   0:00 sleep 6h
hacker        75  0.1  0.0   5240  3840 pts/0    Ss   16:57   0:00 /run/dojo/bin/ssh-entrypoint
hacker        95  0.0  0.0   7868  3200 pts/0    R+   16:58   0:00 ps aux
hacker@processes~killing-processes:~$ kill 73
hacker@processes~killing-processes:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.0  0.0   1056   640 ?        Ss   16:57   0:00 /sbin/docker-init -- /nix/var/nix/profiles/default/bi
root           7  0.0  0.0   5052  2240 ?        S    16:57   0:00 /run/dojo/bin/sleep 6h
hacker        74  0.0  0.0   5052  2560 ?        S    16:57   0:00 sleep 6h
hacker        75  0.0  0.0   5240  3840 pts/0    Ss   16:57   0:00 /run/dojo/bin/ssh-entrypoint
hacker        96  0.0  0.0   7868  3200 pts/0    R+   16:58   0:00 ps aux
hacker@processes~killing-processes:~$ /challenge/run
Great job! Here is your payment:
pwn.college{IovfY8Ri3etSfjuOjZFK9pw8vDm.dJDN4QDLzIzN0czW}
hacker@processes~killing-processes:~$
```
