# Cracking Passwords
In this challenge, we simulate a leak wherein we obtain the passwords stored in `/challenge/shadow-leak` and use it to switch users and run the command.
```
Connected!
hacker@users~cracking-passwords:~$ john /challenge/shadow-leak
Created directory: /home/hacker/.john
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
aardvark         (zardus)
1g 0:00:00:21 100% 2/3 0.04651g/s 270.8p/s 270.8c/s 270.8C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users~cracking-passwords:~$ su zardus
Password:
zardus@users~cracking-passwords:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{Q0vUWD17IaA9Dp5E72dOB9EvDjx.ddTN0UDLzIzN0czW}
zardus@users~cracking-passwords:/home/hacker$
```
