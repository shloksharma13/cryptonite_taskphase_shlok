# Explicit Relative Paths, from /
In this module we learn that `./` is equal to a relative path.
For example, lets say our current directory is `/sys/kernel/` and we want to run `challenge/run` in this directory.
If we use `./challenge/run` or `././challenge/run` it'll be equal to us invoking `challenge/run` because the `./` just means the current directory.
Thus in this challenge we invoke `./challenge/run` which is a relative path to `challenge/run`
This achieves success and unlocks the flag.
```
Connected!
hacker@paths~explicit-relative-paths-from-:~$ /challenge/run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~explicit-relative-paths-from-:~$ cd /
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{8GBRbytvJQwz5y0ePOQPbzdHxo8.dBTN1QDLzIzN0czW}
hacker@paths~explicit-relative-paths-from-:/$
```
