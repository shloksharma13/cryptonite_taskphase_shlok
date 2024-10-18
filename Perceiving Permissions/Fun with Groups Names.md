# Fun with group names
In this challenge we learn about the `id` command which helps us to print the information about the group id and then we use that to change the group and obtain the necessary permissions to read out the flag.
```
Connected!
hacker@permissions~fun-with-groups-names:~$ id
uid=1000(hacker) gid=1000(grp11228) groups=1000(grp11228)
hacker@permissions~fun-with-groups-names:~$ chgrp grp11228 /flag
hacker@permissions~fun-with-groups-names:~$ cat /flag
pwn.college{8iAZuSW4RyPlh00J3NhdM-cCZW-.dJzNyUDLzIzN0czW}
hacker@permissions~fun-with-groups-names:~$
```
