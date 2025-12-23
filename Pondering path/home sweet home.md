# Home Sweet Home
This challenge requires you to access files using  absolute path and a path name in front of /challenge/run
## My Solve
**Flag:** 'pwn.college{gS0gsYr9mopEug7y3LJqd6gfJRf.QXzMDO0wSOwEzNzEzW}'
```
hacker@paths~home-sweet-home:~$ cd /
hacker@paths~home-sweet-home:/$ cd
hacker@paths~home-sweet-home:~$ cd /challenge/run
bash: cd: /challenge/run: Not a directory
hacker@paths~home-sweet-home:~$  /challenge/run
You must provide an argument to /challenge/run when you invoke it!
hacker@paths~home-sweet-home:~$  /challenge/run ~/c
Writing the file to /home/hacker/c!
... and reading it back to you:
pwn.college{gS0gsYr9mopEug7y3LJqd6gfJRf.QXzMDO0wSOwEzNzEzW}

```

## What I Learned
I learned that ~ is shorthand for your home directory, so ~ expands to /home/hacker and ~/x expands to /home/hacker/x.
I also learned that commands like /challenge/run ~/x can require an absolute path, and using ~ still satisfies that because it expands to an absolute path under your home directory.
