# Implicit Relative Paths
In this module we learn about `relative paths`.
Unlike absolute paths, these start from where the directory left off.
Such an example is the given challenge where we're supposed to run `/challenge/run`, but when we run it, the parses displays error and tells us to shift to `/` directory.
So we use `cd /` to shift to the required directory and run `challenge/run` because we're already in the `/` directory, therefore our command to the parse starts from `challenge`
This achieves success and unlocks the flag.
```
Connected!
hacker@paths~implicit-relative-paths-from-:~$ /challenge/run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{MKRO1_VWlRzPX8ueNmoDacBEcVF.dlDN1QDLzIzN0czW}
hacker@paths~implicit-relative-paths-from-:/$
```
