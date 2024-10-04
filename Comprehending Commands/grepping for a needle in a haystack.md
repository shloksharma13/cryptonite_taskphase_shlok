# grepping for a needle in a haystack
In this challenge, we learn about the `grep` command. So we use the `grep` command with the argument `pwn.college` since the key always starts with pwn.college.
This reads out the line in the file that has the word pwn.college. Thus unlocking the key.
```
Connected!
hacker@commands~grepping-for-a-needle-in-a-haystack:~$ grep pwn.college /challenge/data.txt
pwn.college{sHzXy5WnrpK2a2wcqGTP_Jy0lYq.ddTM4QDLzIzN0czW}
hacker@commands~grepping-for-a-needle-in-a-haystack:~$
```
