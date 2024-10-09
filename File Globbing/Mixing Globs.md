# Mixing Globs
In this challenge, we learn about using multiple globs at one. To run `challenging educational and pwning` we notice that they're the only files that start with the respective letters.
So we use the glob `[cep]*` which basically refers to any file that starts with either c or e or p. 
```
Connected!
hacker@globbing~mixing-globs:~$ cd /challenge/files
hacker@globbing~mixing-globs:/challenge/files$ ls
amazing    challenging  educational  great  incredible  kind      magical  optimistic  queenly  splendid   uplifting   wonderful  youthful
beautiful  delightful   fantastic    happy  jovial      laughing  nice     pwning      radiant  thrilling  victorious  xenial     zesty
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run [cep]*
You got it! Here is your flag!
pwn.college{gGPxDEvUl1OWgOjC9j22dYUWzzW.dVjM4QDLzIzN0czW}
hacker@globbing~mixing-globs:/challenge/files$
```
