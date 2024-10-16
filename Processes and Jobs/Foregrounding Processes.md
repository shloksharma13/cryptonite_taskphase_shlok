# Foregrounding Processes
In this challenge, we learn how to foreground a process after it's been shoved into the background.
We start by running `/challenge/run` and then interrupt it with `Ctrl+Z`. We use `bg` to resume it while pushing it in the background and then foregorund it using `fg`.
```
Connected!
hacker@processes~foregrounding-processes:~$ /challenge/run
To pass this level, you need to suspend me, resume the suspended process in the
background, and *then* foreground it without re-suspending it! You can
background me with Ctrl-Z (and resume me in the background with 'bg') or, if
you're not ready to do that for whatever reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~foregrounding-processes:~$ bg
[1]+ /challenge/run &



Yay, I'm now running the background! Because of that, this text will probably
overlap weirdly with the shell prompt. Don't panic; just hit Enter a few times
to scroll this text out. After that, resume me into the foreground with 'fg';
I'll wait.
hacker@processes~foregrounding-processes:~$ fg
/challenge/run
YES! Great job! I'm now running in the foreground. Hit Enter for your flag!

pwn.college{o1eKQHeCvQe-KVfALPYfgfYLABl.dhDN4QDLzIzN0czW}
hacker@processes~foregrounding-processes:~$
```
