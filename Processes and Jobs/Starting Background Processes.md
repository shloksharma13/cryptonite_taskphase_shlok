# Starting Background Processes
In this challenge, we learn that by appending a command with `&` we can open it in the background directly and avoid the suspension and reopening using `bg`.
```
hacker@processes~starting-backgrounded-processes:~$ /challenge/run &
[1] 83



hacker@processes~starting-backgrounded-processes:~$ Yay, you started me in the background! Because of that, this text will probably
overlap weirdly with the shell prompt, but you're used to that by now...

Anyways! Here is your flag!
pwn.college{AWEY6x5Htq3estFATkk6K2Hrks9.dlDN4QDLzIzN0czW}

[1]+  Done                    /challenge/run
hacker@processes~starting-backgrounded-processes:~$
```
