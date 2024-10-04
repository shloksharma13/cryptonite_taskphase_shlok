# hidden files
In this challenge, we are supposed to find a hidden file and read it.
We shift to the `/` directory by using `cd /` command and then display all the files by using `ls -a` command.
Then we use `cat` command with argument `filename` to unlock the flag.
```
root@DESKTOP-BDBALR6:~# ssh -i ./key hacker@dojo.pwn.college
Connected!
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv            bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-32149201655441  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat .flag-32149201655441
pwn.college{oIOaVlE4ulmFXKEncXAuTjm8F7z.dBTN4QDLzIzN0czW}
hacker@commands~hidden-files:/$
```
