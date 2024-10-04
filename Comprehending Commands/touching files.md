In this module we learn about creating files using `touch` command. 
We're supposed to make files `/tmp/pwn` and `tmp/college`.
Therefore we first change the directory to `/tmp` and then use `touch` command once with the argumen `pwn` and next with the argument `college`.
The files are now present in the directory and are checked by `ls`
Now we run `/challenge/run` to unlock the flag.
```
Connected!
hacker@commands~touching-files:~$ cd /tmp
hacker@commands~touching-files:/tmp$ touch pwn
hacker@commands~touching-files:/tmp$ touch college
hacker@commands~touching-files:/tmp$ ls
bin  college  hsperfdata_root  pwn  tmp.XvrUsDZh8M
hacker@commands~touching-files:/tmp$ /challenge/run
Success! Here is your flag:
pwn.college{s3FzgH8-kiRdK9x7tirI9Z0U9WW.dBzM4QDLzIzN0czW}
hacker@commands~touching-files:/tmp$
```
